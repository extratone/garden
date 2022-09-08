---
{"dg-publish":true,"permalink":"/snippets/device/","dgHomeLink":true,"dgPassFrontmatter":false}
---

device

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
-   [Device](device.html)

Class Device
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#device){#device}

Device
======
:::

Drafts defines a single global `device` object which provides access to
information about the current device.

[](#examples){#examples}

### Examples

    // get system info from device object
    var model = device.model;
    var system = device.systemName;
    var osVersion = device.systemVersion;
    var batteryLevel = device.batteryLevel;

    // create and display it in an alert
    var s = "Model: " + model + "\n";
    s = s + "System: " + system + "\n";
    s = s + "OS: " + osVersion + "\n";
    s = s + "Battery: " + batteryLevel;
    alert(s);

    // branch logic based on platform
    if (device.systemName == 'macOS') {
        // do something only on Mac
    }
    else {
        // do something only on iOS
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Device]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [batteryLevel](device.html#batterylevel){.tsd-kind-icon}
-   [model](device.html#model){.tsd-kind-icon}
-   [systemName](device.html#systemname){.tsd-kind-icon}
-   [systemVersion](device.html#systemversion){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#batterylevel .tsd-anchor}

### batteryLevel

::: {.tsd-signature .tsd-kind-icon}
batteryLevel[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [Device.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Device.d.ts#L50)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Current battery level as a number between 0.0 and 1.0
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#model .tsd-anchor}

### model

::: {.tsd-signature .tsd-kind-icon}
model[:]{.tsd-signature-symbol} [\"iPhone\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"iPad\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"Mac\"]{.tsd-signature-type}
:::

-   Defined in
    [Device.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Device.d.ts#L35)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Model of current device.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#systemname .tsd-anchor}

### systemName

::: {.tsd-signature .tsd-kind-icon}
systemName[:]{.tsd-signature-symbol} [\"iOS\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"macOS\"]{.tsd-signature-type}
:::

-   Defined in
    [Device.d.ts:40](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Device.d.ts#L40)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Name of current OS.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#systemversion .tsd-anchor}

### systemVersion

::: {.tsd-signature .tsd-kind-icon}
systemVersion[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Device.d.ts:45](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Device.d.ts#L45)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Version of current OS.
:::
:::
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
-   [Device](device.html){.tsd-kind-icon}
    -   [batteryLevel](device.html#batterylevel){.tsd-kind-icon}
    -   [model](device.html#model){.tsd-kind-icon}
    -   [systemName](device.html#systemname){.tsd-kind-icon}
    -   [systemVersion](device.html#systemversion){.tsd-kind-icon}

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
