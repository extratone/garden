---
{"dg-publish":true,"permalink":"/snippets/reminderlist/","dgHomeLink":true,"dgPassFrontmatter":false}
---

reminderlist

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
-   [ReminderList](reminderlist.html)

Class ReminderList
==================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#reminderlist){#reminderlist}

ReminderList
============
:::

ReminderList objects are used to manipulate and create lists in the
built-in Reminders app.

[](#examples){#examples}

### Examples

    const list = ReminderList.findOrCreate("Groceries");
    let reminder = list.createReminder();
    reminder.title = "Bananas";
    reminder.notes = "Get slightly green ones."
    reminder.update();
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [ReminderList]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [completeTasks](reminderlist.html#completetasks){.tsd-kind-icon}
-   [incompleteTasks](reminderlist.html#incompletetasks){.tsd-kind-icon}
-   [tasks](reminderlist.html#tasks){.tsd-kind-icon}
-   [title](reminderlist.html#title){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [createReminder](reminderlist.html#createreminder){.tsd-kind-icon}
-   [update](reminderlist.html#update){.tsd-kind-icon}
-   [default](reminderlist.html#default){.tsd-kind-icon}
-   [find](reminderlist.html#find){.tsd-kind-icon}
-   [findOrCreate](reminderlist.html#findorcreate){.tsd-kind-icon}
-   [getAllReminderLists](reminderlist.html#getallreminderlists){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#completetasks .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} completeTasks

::: {.tsd-signature .tsd-kind-icon}
completeTasks[:]{.tsd-signature-symbol}
[Reminder](reminder.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [ReminderList.d.ts:32](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L32)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Reminders in the list which have been marked completed.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#incompletetasks .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} incompleteTasks

::: {.tsd-signature .tsd-kind-icon}
incompleteTasks[:]{.tsd-signature-symbol}
[Reminder](reminder.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [ReminderList.d.ts:28](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L28)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Reminders in the list which are NOT completed.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#tasks .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} tasks

::: {.tsd-signature .tsd-kind-icon}
tasks[:]{.tsd-signature-symbol}
[Reminder](reminder.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [ReminderList.d.ts:24](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L24)

::: {.tsd-comment .tsd-typography}
::: {.lead}
All reminders in the list.
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
    [ReminderList.d.ts:20](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L20)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The name of the list.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createreminder .tsd-anchor}

### createReminder

-   createReminder[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Reminder](reminder.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [ReminderList.d.ts:42](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L42)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a new Reminder object in this list
    :::
    :::

    #### Returns [Reminder](reminder.html){.tsd-signature-type} {#returns-reminder .tsd-returns-title}
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
        [ReminderList.d.ts:37](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L37)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Save changes to the list.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#default .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} default

-   default[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[ReminderList](reminderlist.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [ReminderList.d.ts:62](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L62)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Returns the system default reminder list configured for new
    reminders.
    :::
    :::

    #### Returns [ReminderList](reminderlist.html){.tsd-signature-type} {#returns-reminderlist .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#find .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} find

-   find[(]{.tsd-signature-symbol}title[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[ReminderList](reminderlist.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [ReminderList.d.ts:52](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L52)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Searches for a reminder lists matching the title. If none is found,
    return undefined.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### title: [string]{.tsd-signature-type}

    #### Returns [ReminderList](reminderlist.html){.tsd-signature-type} {#returns-reminderlist-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#findorcreate .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} findOrCreate

-   findOrCreate[(]{.tsd-signature-symbol}title[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[ReminderList](reminderlist.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [ReminderList.d.ts:47](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L47)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Searches for a list in the reminders app matching the title. If none
    is found, creates a new list with that title. If more than one list
    with the same name exist in Reminders, the first found will be
    returned.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### title: [string]{.tsd-signature-type}

    #### Returns [ReminderList](reminderlist.html){.tsd-signature-type} {#returns-reminderlist-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#getallreminderlists .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} getAllReminderLists

-   getAllReminderLists[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[ReminderList](reminderlist.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [ReminderList.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ReminderList.d.ts#L57)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get an array all known reminder lists on the device.
    :::
    :::

    #### Returns [ReminderList](reminderlist.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-reminderlist-3 .tsd-returns-title}
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
-   [ReminderList](reminderlist.html){.tsd-kind-icon}
    -   [completeTasks](reminderlist.html#completetasks){.tsd-kind-icon}
    -   [incompleteTasks](reminderlist.html#incompletetasks){.tsd-kind-icon}
    -   [tasks](reminderlist.html#tasks){.tsd-kind-icon}
    -   [title](reminderlist.html#title){.tsd-kind-icon}
    -   [createReminder](reminderlist.html#createreminder){.tsd-kind-icon}
    -   [update](reminderlist.html#update){.tsd-kind-icon}
    -   [default](reminderlist.html#default){.tsd-kind-icon}
    -   [find](reminderlist.html#find){.tsd-kind-icon}
    -   [findOrCreate](reminderlist.html#findorcreate){.tsd-kind-icon}
    -   [getAllReminderLists](reminderlist.html#getallreminderlists){.tsd-kind-icon}

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
