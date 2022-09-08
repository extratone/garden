---
{"dg-publish":true,"permalink":"/snippets/reminder/","dgHomeLink":true,"dgPassFrontmatter":false}
---

reminder

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
-   [Reminder](reminder.html)

Class Reminder
==============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#reminder){#reminder}

Reminder
========
:::

Reminder objects represent individual tasks in a list in the built-in
Reminders app. For examples, see [ReminderList](reminderlist.html)
documentation.
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Reminder]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [alarms](reminder.html#alarms){.tsd-kind-icon}
-   [completionDate](reminder.html#completiondate){.tsd-kind-icon}
-   [dueDate](reminder.html#duedate){.tsd-kind-icon}
-   [dueDateIncludesTime](reminder.html#duedateincludestime){.tsd-kind-icon}
-   [hasAlarms](reminder.html#hasalarms){.tsd-kind-icon}
-   [identifier](reminder.html#identifier){.tsd-kind-icon}
-   [isCompleted](reminder.html#iscompleted){.tsd-kind-icon}
-   [list](reminder.html#list){.tsd-kind-icon}
-   [location](reminder.html#location){.tsd-kind-icon}
-   [notes](reminder.html#notes){.tsd-kind-icon}
-   [priority](reminder.html#priority){.tsd-kind-icon}
-   [startDate](reminder.html#startdate){.tsd-kind-icon}
-   [startDateIncludesTime](reminder.html#startdateincludestime){.tsd-kind-icon}
-   [title](reminder.html#title){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [addAlarm](reminder.html#addalarm){.tsd-kind-icon}
-   [removeAlarms](reminder.html#removealarms){.tsd-kind-icon}
-   [update](reminder.html#update){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#alarms .tsd-anchor}

### alarms

::: {.tsd-signature .tsd-kind-icon}
alarms[:]{.tsd-signature-symbol}
[Alarm](alarm.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [Reminder.d.ts:79](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L79)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The alarms assigned to the reminder, if any.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#completiondate .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} completionDate

::: {.tsd-signature .tsd-kind-icon}
completionDate[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:55](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L55)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Completion date of the reminder. This value is set automatically when
the `isCompleted` property is set to true. Setting this property to
`nil` will set `isCompleted` to false.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#duedate .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} dueDate

::: {.tsd-signature .tsd-kind-icon}
dueDate[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L35)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Due date of the reminder
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#duedateincludestime .tsd-anchor}

### dueDateIncludesTime

::: {.tsd-signature .tsd-kind-icon}
dueDateIncludesTime[:]{.tsd-signature-symbol}
[Boolean]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:40](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L40)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Does the dueDate property include an assigned time. If false,
assignments to the `dueDate` property will ignore time components,
making the reminder due on a specific date without a time assigned.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#hasalarms .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} hasAlarms

::: {.tsd-signature .tsd-kind-icon}
hasAlarms[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:74](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L74)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Returns true if the reminder has any alarms.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#identifier .tsd-anchor}

### identifier

::: {.tsd-signature .tsd-kind-icon}
identifier[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:15](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L15)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Unique identifier for the reminder.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#iscompleted .tsd-anchor}

### isCompleted

::: {.tsd-signature .tsd-kind-icon}
isCompleted[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:69](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L69)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Flag indicating if the task has been completed.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#list .tsd-anchor}

### list

::: {.tsd-signature .tsd-kind-icon}
list[:]{.tsd-signature-symbol}
[ReminderList](reminderlist.html){.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:10](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L10)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The list which this task resides in.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#location .tsd-anchor}

### location

::: {.tsd-signature .tsd-kind-icon}
location[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:30](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L30)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Location of the event.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#notes .tsd-anchor}

### notes

::: {.tsd-signature .tsd-kind-icon}
notes[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:25](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L25)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Notes associated with the event.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#priority .tsd-anchor}

### priority

::: {.tsd-signature .tsd-kind-icon}
priority[:]{.tsd-signature-symbol} [0]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[1]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[5]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[9]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L64)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Integer number representing priority. Assign values matching those Apple
uses as follows:

-   `0`: No priority
-   `1`: High
-   `5`: Medium
-   `9`: Low
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#startdate .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} startDate

::: {.tsd-signature .tsd-kind-icon}
startDate[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:45](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L45)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Start date of the reminder
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#startdateincludestime .tsd-anchor}

### startDateIncludesTime

::: {.tsd-signature .tsd-kind-icon}
startDateIncludesTime[:]{.tsd-signature-symbol}
[Boolean]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L50)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Does the startDate property include an assigned time. If false,
assignments to the `startDate` property will ignore time components,
making the reminder start on a specific date without a time assigned.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#title .tsd-anchor}

### title

::: {.tsd-signature .tsd-kind-icon}
title[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Reminder.d.ts:20](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L20)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The title of the event.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addalarm .tsd-anchor}

### addAlarm

-   addAlarm[(]{.tsd-signature-symbol}alarm[:
    ]{.tsd-signature-symbol}[Alarm](alarm.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Reminder.d.ts:89](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L89)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add an alarm object to the reminder. Be sure to `update()` to save
    after adding alarms. Return `true` if the alarm was successfully
    added. Note that reminders only support alarms created with the
    `Alarm.alarmWithDate` method.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### alarm: [Alarm](alarm.html){.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#removealarms .tsd-anchor}

### removeAlarms

-   removeAlarms[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Reminder.d.ts:94](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L94)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Remove any assigned alarms from the reminder.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#update .tsd-anchor}

### update

-   update[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Reminder.d.ts:84](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Reminder.d.ts#L84)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Save the task. Returns true if the task is successfully saved in
    Reminders.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-1 .tsd-returns-title}
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
-   [Reminder](reminder.html){.tsd-kind-icon}
    -   [alarms](reminder.html#alarms){.tsd-kind-icon}
    -   [completionDate](reminder.html#completiondate){.tsd-kind-icon}
    -   [dueDate](reminder.html#duedate){.tsd-kind-icon}
    -   [dueDateIncludesTime](reminder.html#duedateincludestime){.tsd-kind-icon}
    -   [hasAlarms](reminder.html#hasalarms){.tsd-kind-icon}
    -   [identifier](reminder.html#identifier){.tsd-kind-icon}
    -   [isCompleted](reminder.html#iscompleted){.tsd-kind-icon}
    -   [list](reminder.html#list){.tsd-kind-icon}
    -   [location](reminder.html#location){.tsd-kind-icon}
    -   [notes](reminder.html#notes){.tsd-kind-icon}
    -   [priority](reminder.html#priority){.tsd-kind-icon}
    -   [startDate](reminder.html#startdate){.tsd-kind-icon}
    -   [startDateIncludesTime](reminder.html#startdateincludestime){.tsd-kind-icon}
    -   [title](reminder.html#title){.tsd-kind-icon}
    -   [addAlarm](reminder.html#addalarm){.tsd-kind-icon}
    -   [removeAlarms](reminder.html#removealarms){.tsd-kind-icon}
    -   [update](reminder.html#update){.tsd-kind-icon}

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
