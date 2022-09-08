---
{"dg-publish":true,"permalink":"/snippets/action/","dgHomeLink":true,"dgPassFrontmatter":false}
---

action

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
-   [Action](action.html)

Class Action
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}

module

:   Global

    [](#action){#action}

    Action
    ======

    In addition to being able to lookup an action using the find method,
    a single global `action` object is created and available in scripts
    to inquire about the current action and control flow.

    [](#example){#example}

    ### Example

        // find action
        let action = Action.find("Copy");

        // queue to action to run after the current action
        app.queueAction(action, draft);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Action]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Identification Properties

-   [installURL](action.html#installurl){.tsd-kind-icon}
-   [isSeparator](action.html#isseparator){.tsd-kind-icon}
-   [name](action.html#name){.tsd-kind-icon}
-   [uuid](action.html#uuid){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Query Methods

-   [find](action.html#find){.tsd-kind-icon}
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
    [Action.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Action.d.ts#L35)

::: {.tsd-comment .tsd-typography}
::: {.lead}
URL which can be used to install this Action in another installation of
Drafts. Useful for sharing and backups.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isseparator .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} isSeparator

::: {.tsd-signature .tsd-kind-icon}
isSeparator[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Action.d.ts:47](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Action.d.ts#L47)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If true, the action is a separator.
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
    [Action.d.ts:29](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Action.d.ts#L29)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The display name of the action as displayed in the action list.
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
    [Action.d.ts:41](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Action.d.ts#L41)

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
    ]{.tsd-signature-symbol}[Action](action.html){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Action.d.ts:23](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Action.d.ts#L23)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Search for action matching the name passed and return it if found.
    Useful to lookup and action and queue it to be run using
    `app.queueAction(action, draft)`. This method will return only the
    first found action with the given name, be sure to avoid duplicate
    names in your action list.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Name of a valid, installed action.
        :::

    #### Returns [Action](action.html){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-action-undefined .tsd-returns-title}
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
-   [Action](action.html){.tsd-kind-icon}
    -   [installURL](action.html#installurl){.tsd-kind-icon}
    -   [isSeparator](action.html#isseparator){.tsd-kind-icon}
    -   [name](action.html#name){.tsd-kind-icon}
    -   [uuid](action.html#uuid){.tsd-kind-icon}
    -   [find](action.html#find){.tsd-kind-icon}

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
