# Power BI

## Principles <a href="#reportingprinciples-rules-and-guidelines-principles" id="reportingprinciples-rules-and-guidelines-principles"></a>

### **Keep Data as "Raw" as Possible (Depth)**

Limit (to zero if possible) the number of filters applied to the data source before it is available to a report. This will mean more rows are returned (deep) but will provide more insights into reporting.

{% hint style="danger" %}
**Exception**

Time-based queries, some large data sets will timeout if there are no additional filters added at retrieval time. The only filters that should be applied are time-based filters, e.g. updated in the last 180 days. These filters should be for the largest time frame that allows for the data set to be consistently retrieved without timeout errors.
{% endhint %}

{% hint style="warning" %}
This is somewhat contrary to the best practices given by Microsoft however is required to create meaningful, drillable reports (especially Portfolio Reports).&#x20;
{% endhint %}

### **Keep Data as Slim as Possible (Width)**

Where possible, reduce the number of columns. This will speed up the data collection. If required, create multiple tables and join them via 1:1.

### **Keep Data as Up-to-date as Required**&#x20;

Not all data needs to be updated every day. Having split the data into datasets, we can schedule the refresh of different data at different times.

### **Keep Data Separate and Join at the Last Responsible Moment**

By using DAX to create a "copy" of the data set table, we can create new joins within the reports meaning that data retrieval is quicker.&#x20;

{% hint style="danger" %}
**Exception**

Sometimes, the join is important in order to validate the data quality. By creating the join in the data set, we can further filter data before the report. The joins must be recreated on DAX copy tables, and additionally, joins can be added if required. Note: This can make the report harder to debug.
{% endhint %}

### **Keep Report-specific Logic in Reports**

Filters, calculated columns, measures, summary tables, etc., should be created only within the report. This allows for changes to be made quickly and easily and increases the ability to debug a report. If common logic is required, it should be refactored into a data suite (not a data set).&#x20;

{% hint style="info" %}
You may need to recreate the measures in the report, so naming the measures should take into account that measures names are distinct even when pulled in from other data suites.
{% endhint %}

### **Keep Data in the Best Container for the Data Usage**

Source of truth data should not be tampered with.&#x20;

{% hint style="danger" %}
**Exception**

Sometimes, we require lookup data (or data that affects business logic) that can be updated by end users quickly and easily. This data should be stored in a place that allows for the structure to be maintained but for data to change. Jira look-ups are a good starting place for most Jira data as Administrators can only update them and are in a fixed structure. Google Sheets provide more flexibility, allowing users to enter more complex look-up data, but it can be harder to maintain structure. Understanding the needs of the data entry user and the data requirements of reporting users is required to be able to choose the best container for the data.&#x20;
{% endhint %}

See also: [https://docs.microsoft.com/en-us/power-query/best-practices](https://docs.microsoft.com/en-us/power-query/best-practices)&#x20;
