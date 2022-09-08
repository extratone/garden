---
{"dg-publish":true,"permalink":"/snippets/event/","dgHomeLink":true,"dgPassFrontmatter":false}
---

event

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
-   [Event](event.html)

Class Event
===========
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#event){#event}

Event
=====
:::

Event object represent individual calendar events. For usage examples,
see [Calendar](calendar.html) object documentation.
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Event]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [alarms](event.html#alarms){.tsd-kind-icon}
-   [attendees](event.html#attendees){.tsd-kind-icon}
-   [availability](event.html#availability){.tsd-kind-icon}
-   [calendar](event.html#calendar){.tsd-kind-icon}
-   [creationDate](event.html#creationdate){.tsd-kind-icon}
-   [endDate](event.html#enddate){.tsd-kind-icon}
-   [hasAlarms](event.html#hasalarms){.tsd-kind-icon}
-   [identifier](event.html#identifier){.tsd-kind-icon}
-   [isAllDay](event.html#isallday){.tsd-kind-icon}
-   [lastError](event.html#lasterror){.tsd-kind-icon}
-   [lastModifiedDate](event.html#lastmodifieddate){.tsd-kind-icon}
-   [location](event.html#location){.tsd-kind-icon}
-   [notes](event.html#notes){.tsd-kind-icon}
-   [startDate](event.html#startdate){.tsd-kind-icon}
-   [title](event.html#title){.tsd-kind-icon}
-   [url](event.html#url){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [addAlarm](event.html#addalarm){.tsd-kind-icon}
-   [edit](event.html#edit){.tsd-kind-icon}
-   [removeAllAlarms](event.html#removeallalarms){.tsd-kind-icon}
-   [update](event.html#update){.tsd-kind-icon}
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
    [Event.d.ts:94](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L94)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The alarms assigned to the event, if any.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#attendees .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} attendees

::: {.tsd-signature .tsd-kind-icon}
attendees[:]{.tsd-signature-symbol}
[Object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [Event.d.ts:75](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L75)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Attendees of the event as an array of objects in the format:
:::

    {
       "isCurrentUser": false,
       "name": "John Appleseed",
       "status": "accepted",
       "type": "person",
       "role": "required"
    }
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#availability .tsd-anchor}

### availability

::: {.tsd-signature .tsd-kind-icon}
availability[:]{.tsd-signature-symbol} [\"busy\"]{.tsd-signature-type}[
\| ]{.tsd-signature-symbol}[\"free\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"tentative\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"unavailable\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"notSupported\"]{.tsd-signature-type}
:::

-   Defined in
    [Event.d.ts:80](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L80)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Availability for scheduling. Not supported by all Calendar servers.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#calendar .tsd-anchor}

### calendar

::: {.tsd-signature .tsd-kind-icon}
calendar[:]{.tsd-signature-symbol}
[Calendar](calendar.html){.tsd-signature-type}
:::

-   Defined in
    [Event.d.ts:10](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L10)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The calendar which this event resides in.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#creationdate .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} creationDate

::: {.tsd-signature .tsd-kind-icon}
creationDate[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Event.d.ts:55](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L55)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Original creation date of the event.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#enddate .tsd-anchor}

### endDate

::: {.tsd-signature .tsd-kind-icon}
endDate[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Event.d.ts:40](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L40)

::: {.tsd-comment .tsd-typography}
::: {.lead}
End date of the event.
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
    [Event.d.ts:89](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L89)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Returns true if the event has any alarms.
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
    [Event.d.ts:15](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L15)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Unique identifier for the event
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isallday .tsd-anchor}

### isAllDay

::: {.tsd-signature .tsd-kind-icon}
isAllDay[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Event.d.ts:45](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L45)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Flag for all day events.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lasterror .tsd-anchor}

### lastError

::: {.tsd-signature .tsd-kind-icon}
lastError[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}
:::

-   Defined in
    [Event.d.ts:99](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L99)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function fails, this property will contain the last error as a
string message, otherwise it will be `undefined`.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lastmodifieddate .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} lastModifiedDate

::: {.tsd-signature .tsd-kind-icon}
lastModifiedDate[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Event.d.ts:60](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L60)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Last change to the event.
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
    [Event.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L50)

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
    [Event.d.ts:25](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L25)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Notes associated with the event.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#startdate .tsd-anchor}

### startDate

::: {.tsd-signature .tsd-kind-icon}
startDate[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Event.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L35)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Start date of the event.
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
    [Event.d.ts:20](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L20)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The title of the event.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#url .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} url

::: {.tsd-signature .tsd-kind-icon}
url[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Event.d.ts:30](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L30)

::: {.tsd-comment .tsd-typography}
::: {.lead}
URL associated with the event. Setting URL value will fail if the value
is not a valid URL.
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
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Event.d.ts:114](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L114)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add an alarm object to the event. Be sure to `update()` to save
    after adding alarms.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### alarm: [Alarm](alarm.html){.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#edit .tsd-anchor}

### edit

-   edit[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Event.d.ts:109](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L109)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open the event in the system event editing card. The user will be
    able to modify/edit the event values and add to a calendar from this
    view. Returns true if the event was saved, false if the user
    canceled or deleted the event.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#removeallalarms .tsd-anchor}

### removeAllAlarms

-   removeAllAlarms[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Event.d.ts:119](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L119)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Remove any assigned alarms from the event.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-1 .tsd-returns-title}
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
        [Event.d.ts:104](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Event.d.ts#L104)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Save the event. Returns true if the event is successfully saved in
    Calendars.
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
-   [Event](event.html){.tsd-kind-icon}
    -   [alarms](event.html#alarms){.tsd-kind-icon}
    -   [attendees](event.html#attendees){.tsd-kind-icon}
    -   [availability](event.html#availability){.tsd-kind-icon}
    -   [calendar](event.html#calendar){.tsd-kind-icon}
    -   [creationDate](event.html#creationdate){.tsd-kind-icon}
    -   [endDate](event.html#enddate){.tsd-kind-icon}
    -   [hasAlarms](event.html#hasalarms){.tsd-kind-icon}
    -   [identifier](event.html#identifier){.tsd-kind-icon}
    -   [isAllDay](event.html#isallday){.tsd-kind-icon}
    -   [lastError](event.html#lasterror){.tsd-kind-icon}
    -   [lastModifiedDate](event.html#lastmodifieddate){.tsd-kind-icon}
    -   [location](event.html#location){.tsd-kind-icon}
    -   [notes](event.html#notes){.tsd-kind-icon}
    -   [startDate](event.html#startdate){.tsd-kind-icon}
    -   [title](event.html#title){.tsd-kind-icon}
    -   [url](event.html#url){.tsd-kind-icon}
    -   [addAlarm](event.html#addalarm){.tsd-kind-icon}
    -   [edit](event.html#edit){.tsd-kind-icon}
    -   [removeAllAlarms](event.html#removeallalarms){.tsd-kind-icon}
    -   [update](event.html#update){.tsd-kind-icon}

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
