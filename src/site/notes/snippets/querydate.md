---
{"dg-publish":true,"permalink":"/snippets/querydate/","dgHomeLink":true,"dgPassFrontmatter":false}
---

querydate

::: {.tsd-page-toolbar}
::: {.container}
::: {.table-wrap}
::: {#tsd-search .table-cell index="../assets/js/search.json" base=".."}
::: {.field}
Search
:::

-   Preparing search index\...
-   The search index is not available

[Drafts Script Reference](../index.html){.title}
:::

::: {#tsd-widgets .table-cell}
::: {#tsd-filter}
[Options](#){.tsd-widget .options .no-caption}

::: {.tsd-filter-group}
::: {#tsd-filter-visibility .tsd-select}
[All]{.tsd-select-label}

-   Public
-   Public/Protected
-   All
:::

Inherited Only exported
:::
:::

[Menu](#){.tsd-widget .menu .no-caption}
:::
:::
:::
:::

::: {.tsd-page-title}
::: {.container}
-   [Globals](../globals.html)
-   [QueryDate](querydate.html)

Class QueryDate
===============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#querydate){#querydate}

QueryDate
=========
:::

Represents a dynamic date for use in queries. `QueryDate` is used when
configuring [Workspace](workspace.html) objects `startDate` and
`endDate` properties.

QueryDates always specify a date with time components being ignored. If
used a the start of a query range, the time will be moved to the
beginning of that day. If used at the end of a query range, time will be
moved to the end of that day.

[](#example-create-workspace-with-date-range){#example-create-workspace-with-date-range}

### Example: Create Workspace with date range

    // create a workspace
    let workspace = new Workspace();

    // create a QueryDate for three days ago
    let start = new QueryDate();
    start.field = "created"
    start.type = "relative"
    start.days = -3;

    // create a QueryDate for specific date
    let qDate = new QueryDate();
    qDate.field = "modified"
    qDate.type = "absolute"
    qDate.date = Date.today();

    // assign to the workspace and apply
    workspace.startDate = start; // .endDate also available
    app.applyWorkspace(workspace);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [QueryDate]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](querydate.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [date](querydate.html#date){.tsd-kind-icon}
-   [days](querydate.html#days){.tsd-kind-icon}
-   [field](querydate.html#field){.tsd-kind-icon}
-   [type](querydate.html#type){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [create](querydate.html#create){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Constructors
------------

::: {.section .tsd-panel .tsd-member .tsd-kind-constructor .tsd-parent-kind-class}
[]{#constructor .tsd-anchor}

### constructor

-   new QueryDate[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[QueryDate](querydate.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [QueryDate.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/QueryDate.d.ts#L57)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a new instance.
    :::
    :::

    #### Returns [QueryDate](querydate.html){.tsd-signature-type} {#returns-querydate .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#date .tsd-anchor}

### date

::: {.tsd-signature .tsd-kind-icon}
date[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [QueryDate.d.ts:52](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/QueryDate.d.ts#L52)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Absolute date to use when evaluating the query dates of \"absolute\"
type.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#days .tsd-anchor}

### days

::: {.tsd-signature .tsd-kind-icon}
days[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [QueryDate.d.ts:47](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/QueryDate.d.ts#L47)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Integer number of days to when evaluating query dates of \"relative\".
This value can be negative. For example, a \"relative\" type with \"-3\"
days, will always evaluated to 3 days ago when the query is run.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#field .tsd-anchor}

### field

::: {.tsd-signature .tsd-kind-icon}
field[:]{.tsd-signature-symbol}
[queryDateField](../globals.html#querydatefield){.tsd-signature-type}
:::

-   Defined in
    [QueryDate.d.ts:37](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/QueryDate.d.ts#L37)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The date field to use when querying
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#type .tsd-anchor}

### type

::: {.tsd-signature .tsd-kind-icon}
type[:]{.tsd-signature-symbol}
[queryDateType](../globals.html#querydatetype){.tsd-signature-type}
:::

-   Defined in
    [QueryDate.d.ts:42](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/QueryDate.d.ts#L42)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The type of date range. \"relative\" dates use the `days` property to
add days to the current date when evaluating a query. \"absolute\" type
query dates use the `date` property for a specific day.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Workspace](workspace.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [QueryDate.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/QueryDate.d.ts#L57)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a new instance.
    :::
    :::

    #### Returns [Workspace](workspace.html){.tsd-signature-type} {#returns-workspace .tsd-returns-title}
:::
:::
:::

::: {.col-4 .col-menu .menu-sticky-wrap .menu-highlight}
-   [*Globals*](../globals.html)

```{=html}
<!-- -->
```

```{=html}
<!-- -->
```
-   [QueryDate](querydate.html){.tsd-kind-icon}
    -   [constructor](querydate.html#constructor){.tsd-kind-icon}
    -   [date](querydate.html#date){.tsd-kind-icon}
    -   [days](querydate.html#days){.tsd-kind-icon}
    -   [field](querydate.html#field){.tsd-kind-icon}
    -   [type](querydate.html#type){.tsd-kind-icon}
    -   [create](querydate.html#create){.tsd-kind-icon}

```{=html}
<!-- -->
```
:::
:::
:::

::: {.container}
Legend
------

::: {.tsd-legend-group}
-   [Constructor]{.tsd-kind-icon}
-   [Property]{.tsd-kind-icon}
-   [Method]{.tsd-kind-icon}

```{=html}
<!-- -->
```
-   [Property]{.tsd-kind-icon}

```{=html}
<!-- -->
```
-   [Static method]{.tsd-kind-icon}
:::
:::

::: {.container .tsd-generator}
Generated using [TypeDoc](https://typedoc.org/)
:::

::: {.overlay}
:::
