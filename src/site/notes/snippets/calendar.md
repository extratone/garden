---
{"dg-publish":true,"permalink":"/snippets/calendar/","dgHomeLink":true,"dgPassFrontmatter":false}
---

calendar

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
-   [Calendar](calendar.html)

Class Calendar
==============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#calendar){#calendar}

Calendar
========
:::

Calendar objects are used to manipulate and create calendars in the
built-in Calendars app and its associated accounts.

[](#example-event-creation){#example-event-creation}

#### Example: Event Creation

    var calendar = Calendar.findOrCreate("Activities");
    var event = calendar.createEvent();
    event.title = "Dinner Party";
    event.notes = "Bring side dish.";
    event.startDate = Date.parse("7pm next friday");
    event.endDate = Date.parse("10pm next friday");
    event.isAllDay = false;
    if (!event.update()) {
      console.log(event.lastError);
    }

[](#example-reading-calendar-events){#example-reading-calendar-events}

Example: Reading Calendar Events
================================

    // load a calendar
    let cal = Calendar.find("Test");
    // loop over events in the last 30 days and alert the name of each.
    if (cal) {
        let events = cal.events((30).days().ago(), new Date());
        for (let event of events) {
            alert(event.title);
        }
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Calendar]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [allowsContentModificationx](calendar.html#allowscontentmodificationx){.tsd-kind-icon}
-   [isImmutable](calendar.html#isimmutable){.tsd-kind-icon}
-   [title](calendar.html#title){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [createEvent](calendar.html#createevent){.tsd-kind-icon}
-   [events](calendar.html#events){.tsd-kind-icon}
-   [update](calendar.html#update){.tsd-kind-icon}
-   [default](calendar.html#default){.tsd-kind-icon}
-   [find](calendar.html#find){.tsd-kind-icon}
-   [findOrCreate](calendar.html#findorcreate){.tsd-kind-icon}
-   [getAllCalendars](calendar.html#getallcalendars){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#allowscontentmodificationx .tsd-anchor}

### allowsContentModificationx

::: {.tsd-signature .tsd-kind-icon}
allowsContentModificationx[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [Calendar.d.ts:40](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L40)

::: {.tsd-comment .tsd-typography}
::: {.lead}
A Boolean value that indicates whether you can add, edit, and delete
items in the calendar.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isimmutable .tsd-anchor}

### isImmutable

::: {.tsd-signature .tsd-kind-icon}
isImmutable[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Calendar.d.ts:44](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L44)

::: {.tsd-comment .tsd-typography}
::: {.lead}
A Boolean value indicating whether the calendar's properties can be
edited or deleted.
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
    [Calendar.d.ts:36](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L36)
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createevent .tsd-anchor}

### createEvent

-   createEvent[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Event](event.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Calendar.d.ts:54](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L54)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a new Event object in this calendar.
    :::
    :::

    #### Returns [Event](event.html){.tsd-signature-type} {#returns-event .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#events .tsd-anchor}

### events

-   events[(]{.tsd-signature-symbol}startDate[:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}, endDate[:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Event](event.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Calendar.d.ts:59](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L59)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Returns array of events on the calendar between the start and end
    dates specified.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### startDate: [Date]{.tsd-signature-type}

    -   ##### endDate: [Date]{.tsd-signature-type}

    #### Returns [Event](event.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-event-1 .tsd-returns-title}
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
        [Calendar.d.ts:49](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L49)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Save changes to the calendar.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#default .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} default

-   default[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Calendar](calendar.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Calendar.d.ts:79](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L79)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Returns the system default calendar configured for new events.
    :::
    :::

    #### Returns [Calendar](calendar.html){.tsd-signature-type} {#returns-calendar .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#find .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} find

-   find[(]{.tsd-signature-symbol}title[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Calendar](calendar.html){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Calendar.d.ts:69](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L69)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Searches for a calendar matching the title. If none is found, return
    `undefined`.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### title: [string]{.tsd-signature-type}

    #### Returns [Calendar](calendar.html){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-calendar-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#findorcreate .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} findOrCreate

-   findOrCreate[(]{.tsd-signature-symbol}title[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Calendar](calendar.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Calendar.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L64)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Searches for a calendar matching the title. If none is found,
    creates a new list with that title in your default calendars
    account. If more than one calendar with the same name exist in
    Calendars, the first found will be returned.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### title: [string]{.tsd-signature-type}

    #### Returns [Calendar](calendar.html){.tsd-signature-type} {#returns-calendar-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#getallcalendars .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} getAllCalendars

-   getAllCalendars[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Calendar](calendar.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Calendar.d.ts:74](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Calendar.d.ts#L74)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get an array all known calendars on the device.
    :::
    :::

    #### Returns [Calendar](calendar.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-calendar-2 .tsd-returns-title}
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
-   [Calendar](calendar.html){.tsd-kind-icon}
    -   [allowsContentModificationx](calendar.html#allowscontentmodificationx){.tsd-kind-icon}
    -   [isImmutable](calendar.html#isimmutable){.tsd-kind-icon}
    -   [title](calendar.html#title){.tsd-kind-icon}
    -   [createEvent](calendar.html#createevent){.tsd-kind-icon}
    -   [events](calendar.html#events){.tsd-kind-icon}
    -   [update](calendar.html#update){.tsd-kind-icon}
    -   [default](calendar.html#default){.tsd-kind-icon}
    -   [find](calendar.html#find){.tsd-kind-icon}
    -   [findOrCreate](calendar.html#findorcreate){.tsd-kind-icon}
    -   [getAllCalendars](calendar.html#getallcalendars){.tsd-kind-icon}

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
