# End User Best Practice

## Releases / Versions

Further reading:

What is a version? | Jira Software Cloud | Atlassian Support

Note

Jira swaps releases and versions depending on the page that you are looking at.

Why

By tagging issues with a release, we can obliviously get list of items that are released within a version. But, as after we release a version, we can then use the “affectedVersion” field to attach defects and bugs. This then becomes a measure of quality - too many defects against a release may show us a slip in practice or that something was missed, if nothing else it shows that something can be improved.

Release notes

The created confluence page has the Jira issues widget automatically set up.

Name Convention

Prefix: Identifier

Where prefix is either Release or Milestone.

If “release” then the identifier should indicate either a version, a month, or a change request number.

If “milestone” then the identifier should indicate what the milestone represents.

Examples

“Milestone: Funding Approval”

“Release: V1.0”

“Release: September 2022”

“Release: CR-39034”

The related work of the release should provide more information (through a confluence page). For example, the change request details:

Configuration

Advanced Roadmaps

Releases are shown as circles on the top of the roadmaps and can be highlighted on the timeline.



## Components

Further Reading:

What are components? | Jira Software Cloud | Atlassian Support

How to use Jira Components - Tips and Best Practic... - Atlassian Community

Why

Using the component field for system components allows for quick change management.

The component page shows how many issues are assigned to each component giving us an idea of how much change is occurring within at the area.

The description can be a URL linking to a confluence page - unfortunately the URL is not shown as a hyperlink, but chrome/edge gives the ability to open by highlighting and right clicking. The confluence page is a good idea as it can provide much more details, diagrams, links to other pages and resources and reports.

Jira shows all issues assigned to the component - unfortunately it shows all items not just open items but clicking on the issues link presents the search field where status can be added to the filter. A confluence page can easily be set up to provide this information also.

Component lead is a great short-cut to knowing who the “go to person” is for a given area. And the “default assignee” field allows for newly created issues identified within the component to be automatically assigned to the right person.

Naming Convention

System - Container (xN) - Component

Examples:

Apparel 21 - ERP - Database

For more detail see The C4 model for visualising software architecture

Configuration

Roadmaps

Releases (or Versions) are shown as quick filters in the roadmaps
