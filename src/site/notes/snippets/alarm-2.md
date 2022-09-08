---
{"dg-publish":true,"permalink":"/snippets/alarm-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

alarm-2

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
-   [Alarm](alarm.html)

Class Alarm
===========
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#alarm){#alarm}

Alarm
=====
:::

Alarms are alerts which can be attached to [Reminder](reminder.html) and
[Event](event.html) objects.

[](#examples){#examples}

### Examples

    let list = ReminderList.findOrCreate("Errands");
    let reminder = list.createReminder();
    reminder.title = "Get more paper towels";

    let alarm = Alarm.alarmWithDate((3).days().fromNow());
    reminder.addAlarm(alarm);
    reminder.update();
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Alarm]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Methods

-   [alarmWithDate](alarm.html#alarmwithdate){.tsd-kind-icon}
-   [alarmWithOffset](alarm.html#alarmwithoffset){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#alarmwithdate .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} alarmWithDate

-   alarmWithDate[(]{.tsd-signature-symbol}date[:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Alarm](alarm.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Alarm.d.ts:24](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Alarm.d.ts#L24)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Alarm set to remind at a specific date/time.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### date: [Date]{.tsd-signature-type}

    #### Returns [Alarm](alarm.html){.tsd-signature-type} {#returns-alarm .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#alarmwithoffset .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} alarmWithOffset

-   alarmWithOffset[(]{.tsd-signature-symbol}seconds[:
    ]{.tsd-signature-symbol}[Number]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Alarm](alarm.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Alarm.d.ts:30](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Alarm.d.ts#L30)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Alarm set to remind at a specific number of seconds relative to the
    start date of the event. Note that alarms created with this methods
    are only supported on [Event](event.html) objects, not
    [Reminder](reminder.html) objects.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### seconds: [Number]{.tsd-signature-type}

    #### Returns [Alarm](alarm.html){.tsd-signature-type} {#returns-alarm-1 .tsd-returns-title}
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
-   [Alarm](alarm.html){.tsd-kind-icon}
    -   [alarmWithDate](alarm.html#alarmwithdate){.tsd-kind-icon}
    -   [alarmWithOffset](alarm.html#alarmwithoffset){.tsd-kind-icon}

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
