---
{"dg-publish":true,"permalink":"/snippets/actiongroup/","dgHomeLink":true,"dgPassFrontmatter":false}
---

actiongroup

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
-   [ActionGroup](actiongroup.html)

Class ActionGroup
=================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#actiongroup){#actiongroup}

ActionGroup
===========
:::

Represents an action group. Can be used to inquire and load action
groups in the action list and action bar using methods on the
[App](app.html) object.

[](#examples){#examples}

### Examples

    let group = ActionGroup.find("Basic");
    app.loadActionGroup(group);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [ActionGroup]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Content Properties

-   [actions](actiongroup.html#actions){.tsd-kind-icon}

### Identification Properties

-   [installURL](actiongroup.html#installurl){.tsd-kind-icon}
-   [name](actiongroup.html#name){.tsd-kind-icon}
-   [uuid](actiongroup.html#uuid){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Query Methods

-   [find](actiongroup.html#find){.tsd-kind-icon}
-   [getAll](actiongroup.html#getall){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Content Properties
------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#actions .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} actions

::: {.tsd-signature .tsd-kind-icon}
actions[:]{.tsd-signature-symbol}
[Action](action.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [ActionGroup.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionGroup.d.ts#L50)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The actions contained in the action group.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Identification Properties
-------------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#installurl .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} installURL

::: {.tsd-signature .tsd-kind-icon}
installURL[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [ActionGroup.d.ts:44](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionGroup.d.ts#L44)

::: {.tsd-comment .tsd-typography}
::: {.lead}
URL which can be used to install this Action Group in another
installation of Drafts. Useful for sharing and backups.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#name .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} name

::: {.tsd-signature .tsd-kind-icon}
name[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [ActionGroup.d.ts:32](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionGroup.d.ts#L32)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The display name of the action group.
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
    [ActionGroup.d.ts:38](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionGroup.d.ts#L38)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The unique identifier of the action group.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Query Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#find .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} find

-   find[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[ActionGroup](actiongroup.html){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [ActionGroup.d.ts:26](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionGroup.d.ts#L26)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Search for action group matching the name passed and return it if
    found. Returns `undefined` if not found.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The display name of the action group.
        :::

    #### Returns [ActionGroup](actiongroup.html){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-actiongroup-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#getall .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} getAll

-   getAll[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[ActionGroup](actiongroup.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [ActionGroup.d.ts:19](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ActionGroup.d.ts#L19)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get list of all available action groups.
    :::
    :::

    #### Returns [ActionGroup](actiongroup.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-actiongroup .tsd-returns-title}
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
-   [ActionGroup](actiongroup.html){.tsd-kind-icon}
    -   [actions](actiongroup.html#actions){.tsd-kind-icon}
    -   [installURL](actiongroup.html#installurl){.tsd-kind-icon}
    -   [name](actiongroup.html#name){.tsd-kind-icon}
    -   [uuid](actiongroup.html#uuid){.tsd-kind-icon}
    -   [find](actiongroup.html#find){.tsd-kind-icon}
    -   [getAll](actiongroup.html#getall){.tsd-kind-icon}

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
