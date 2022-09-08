---
{"dg-publish":true,"permalink":"/snippets/actionlog/","dgHomeLink":true,"dgPassFrontmatter":false}
---

actionlog

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
-   [ActionLog](actionlog.html)

Class ActionLog
===============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#actionlog){#actionlog}

ActionLog
=========
:::

ActionLog objects represent entries in the [action log](). ActionLog
objects are accessed using the `actionLogs` property of the
[Draft](draft.html) object.

    // loop over log entries, deleting any more than 100 days old
    for(let log of draft.actionLogs) {
      if (log.executedAt < Date.today.addDays(-100)) {
        log.delete();
      }
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [ActionLog]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Content Properties

-   [executedAt](actionlog.html#executedat){.tsd-kind-icon}
-   [executedDevice](actionlog.html#executeddevice){.tsd-kind-icon}
-   [executedLatitude](actionlog.html#executedlatitude){.tsd-kind-icon}
-   [executedLongitude](actionlog.html#executedlongitude){.tsd-kind-icon}
-   [log](actionlog.html#log){.tsd-kind-icon}
-   [status](actionlog.html#status){.tsd-kind-icon}

### Identification Properties

-   [action](actionlog.html#action){.tsd-kind-icon}
-   [draft](actionlog.html#draft){.tsd-kind-icon}
-   [uuid](actionlog.html#uuid){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [delete](actionlog.html#delete){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Content Properties
------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#executedat .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} executedAt

::: {.tsd-signature .tsd-kind-icon}
executedAt[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [ActionLog.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L35)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Timestamp for the creation of the log entry
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#executeddevice .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} executedDevice

::: {.tsd-signature .tsd-kind-icon}
executedDevice[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [ActionLog.d.ts:60](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L60)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Which device the action was performed on, typically \'iPhone\',
\'iPad\', or \'Mac\'
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#executedlatitude .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} executedLatitude

::: {.tsd-signature .tsd-kind-icon}
executedLatitude[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [ActionLog.d.ts:55](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L55)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The latitude portion of the location recorded when action was executed,
if location services are enabled.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#executedlongitude .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} executedLongitude

::: {.tsd-signature .tsd-kind-icon}
executedLongitude[:]{.tsd-signature-symbol}
[number]{.tsd-signature-type}
:::

-   Defined in
    [ActionLog.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L50)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The longitude portion of the location recorded when action was executed,
if location services are enabled.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#log .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} log

::: {.tsd-signature .tsd-kind-icon}
log[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [ActionLog.d.ts:25](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L25)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The content of the log
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#status .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} status

::: {.tsd-signature .tsd-kind-icon}
status[:]{.tsd-signature-symbol} [\"pending\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"in-progress\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"completed\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"failed\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"cancelled\"]{.tsd-signature-type}
:::

-   Defined in
    [ActionLog.d.ts:30](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L30)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Status of the log. \"failed\" indicates the action ended in an error,
\"completed\" indicates successful completion of the action.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Identification Properties
-------------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#action .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} [Readonly]{.tsd-flag .ts-flagReadonly} action

::: {.tsd-signature .tsd-kind-icon}
action[:]{.tsd-signature-symbol}
[Action](action.html){.tsd-signature-type}
:::

-   Defined in
    [ActionLog.d.ts:45](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L45)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The [Action](action.html) object related to the log. This value may be
nil if the action no longer exists.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#draft .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} [Readonly]{.tsd-flag .ts-flagReadonly} draft

::: {.tsd-signature .tsd-kind-icon}
draft[:]{.tsd-signature-symbol} [Draft](draft.html){.tsd-signature-type}
:::

-   Defined in
    [ActionLog.d.ts:40](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L40)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The [Draft](draft.html) object related to the log. This value may be nil
if the action was performed without a draft in context, or if the
related draft no longer exists.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#uuid .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} uuid

::: {.tsd-signature .tsd-kind-icon}
uuid[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [ActionLog.d.ts:20](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L20)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Unique identifier
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#delete .tsd-anchor}

### delete

-   delete[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [ActionLog.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionLog.d.ts#L64)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Delete the action log. This is permanent and should be used with
    caution
    :::
    :::

    #### Returns [any]{.tsd-signature-type} {#returns-any .tsd-returns-title}
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
-   [ActionLog](actionlog.html){.tsd-kind-icon}
    -   [action](actionlog.html#action){.tsd-kind-icon}
    -   [draft](actionlog.html#draft){.tsd-kind-icon}
    -   [executedAt](actionlog.html#executedat){.tsd-kind-icon}
    -   [executedDevice](actionlog.html#executeddevice){.tsd-kind-icon}
    -   [executedLatitude](actionlog.html#executedlatitude){.tsd-kind-icon}
    -   [executedLongitude](actionlog.html#executedlongitude){.tsd-kind-icon}
    -   [log](actionlog.html#log){.tsd-kind-icon}
    -   [status](actionlog.html#status){.tsd-kind-icon}
    -   [uuid](actionlog.html#uuid){.tsd-kind-icon}
    -   [delete](actionlog.html#delete){.tsd-kind-icon}

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
