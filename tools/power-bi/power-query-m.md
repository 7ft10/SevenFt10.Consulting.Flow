# Power Query M

## Useful Functions

### fnGetDefaultHeaders

{% hint style="info" %}
For cloud-based Jira Password is the API Key
{% endhint %}

```powerquery
() =>
[
    #"Content-Type" = "application/json",
    #"Authorization" = "Basic " & Binary.ToText(Text.ToBinary(Username & ":" & Password), 0),
    #"Retry-After" = "120"
]
```

### fnTypeTableColumns

```powerquery
(tableToType as table, optional fieldsAndSchemaTypes as table, optional testCount as number) as table =>  
	List.Accumulate(Table.ColumnNames(tableToType), tableToType, (s, c) =>
  try
    let 
      schemaType = 
        if (fieldsAndSchemaTypes <> null) then
          try Table.SelectRows(fieldsAndSchemaTypes, each [name] = c)[#"schema type"]{0} otherwise null
        else 
          null,
      tests = List.Buffer(List.FirstN(Table.Column(s, c), if (testCount = null) then 100 else testCount)),
      fieldType = 
        if (schemaType = "string") then type text
        else if (schemaType = "number") then Int64.Type
        else null
    in
      if (fieldType <> null) then 
        Table.TransformColumnTypes(s, {{c, fieldType}})
      else  
        // Already has a defined column type
        if (Expression.Evaluate("type "& Table.SelectRows(Table.Schema(s), each [Name] = c){0}[Kind]) <> type any) then
          s
      
        // All null values then make text type, unless it has a schema type we can deal with 
        else if (List.MatchesAll(tests, each _ = null)) then
          try 
            if (schemaType = "date") then Table.TransformColumnTypes(s, {{c, type date}})            
            else if (schemaType = "datetime") then Table.TransformColumnTypes(s, {{c, type datetime}})
            else Table.TransformColumnTypes(s, {{c, type text}})
          otherwise 
            Table.TransformColumnTypes(s, {{c, type text}})  
        
        // Logic Types
        else if (List.MatchesAll(tests, each _ = null or (try _ = false or _ = true or Text.Upper(Text.From(_)) = "FALSE" or Text.Upper(Text.From(_)) = "TRUE" otherwise false))) then
          Table.TransformColumnTypes(s, {{c, type logical}})
        
        // Number Types
        else if (List.MatchesAll(tests, each _ = null or (try Number.Mod(Number.From(_), 1) otherwise -1) = 0)) then
          Table.TransformColumnTypes(s, {{c, Int64.Type}})
        else if (List.MatchesAll(tests, each _ = null or (try Number.Mod(Number.From(_) + 0.1, 1) otherwise -1) > 0)) then
          Table.TransformColumnTypes(s, {{c, type number}})
        
        // Date Types
        else if (List.MatchesAll(tests, each _ = null or (try Date.Year(Date.From(_)) > 2000 otherwise false))) then
          Table.TransformColumnTypes(s, {{c, type date}})
        else if (List.MatchesAll(tests, each _ = null or (try Date.Year(DateTime.Date(DateTime.From(_))) > 2000 otherwise false))) then
          Table.TransformColumnTypes(s, {{c, type datetime}})
        else if (List.MatchesAll(tests, each _ = null or (try Date.Year(DateTime.Date(DateTimeZone.RemoveZone(DateTimeZone.From(_)))) > 2000 otherwise false))) then
          //Table.TransformColumnTypes(s, {{c, type datetimezone}}) // datetimezone becomes text when surfaced to datamart - why M$ why!
          Table.TransformColumnTypes(Table.TransformColumnTypes(s, {{c, type datetimezone}}), {{c, type datetime}})

        // Else 
        else
          try 
            if (schemaType = "date") then Table.TransformColumnTypes(s, {{c, type date}})            
            else if (schemaType = "datetime") then Table.TransformColumnTypes(s, {{c, type datetime}})
            else Table.TransformColumnTypes(s, {{c, type text}})
          otherwise 
            Table.TransformColumnTypes(s, {{c, type text}})  
  otherwise 
    s
  )
```

### fnSortTableColumns

```powerquery
(tableToSort as table) as table =>
  Table.ReorderColumns(tableToSort,
    let
      alphaSort = List.Buffer(List.Sort(Table.ColumnNames(tableToSort), Order.Ascending)),
      keyFixedLower = if List.Contains(alphaSort, "Key") then { "Key" } & List.RemoveItems(alphaSort, { "Key" }) else alphaSort,
      keyFixed = if List.Contains(keyFixedLower, "key") then { "key" } & List.RemoveItems(keyFixedLower, { "key" }) else keyFixedLower,
      idFixed = if List.Contains(keyFixed, "Id") then { "Id" } & List.RemoveItems(keyFixed, { "Id" }) else keyFixed,
      idFixedLower = if List.Contains(idFixed, "id") then { "id" } & List.RemoveItems(idFixed, { "id" }) else idFixed
    in
      idFixedLower,
    MissingField.Ignore
  )
```

### fnExpandedColumnsFancy

```powerquery
(tableToFix as table, optional testCount as number) as table =>
    List.Accumulate(Table.ColumnNames(tableToFix), tableToFix, (s, c) =>
        let 
            tests = List.Buffer(List.FirstN(List.RemoveNulls(List.FirstN(Table.Column(s, c), if (testCount = null) then 5000 else testCount * 5)), if (testCount = null) then 1000 else testCount))
        in
            if (List.MatchesAny(tests, each try _ is record otherwise false)) then
                if (List.MatchesAny(tests, each try Record.HasFields(_, "id") and Record.HasFields(_, "name") otherwise false)) then
                    Table.ExpandRecordColumn(s, c, {"id", "name" }, { c & " Id", c})
                else if (List.MatchesAny(tests, each try Record.HasFields(_, "id") and Record.HasFields(_, "value") otherwise false)) then
                    Table.ExpandRecordColumn(s, c, {"id", "value" }, { c & " Id", c})
                else if (List.MatchesAny(tests, each try Record.HasFields(_, "key") and Record.HasFields(_, "name") otherwise false)) then
                    Table.ExpandRecordColumn(s, c, {"key", "name" }, { c & " Key", c})
                else 
                    s
            else 
                s
    )
```

