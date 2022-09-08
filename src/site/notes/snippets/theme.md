---
{"dg-publish":true,"permalink":"/snippets/theme/","dgHomeLink":true,"dgPassFrontmatter":false}
---

theme

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
-   [Theme](theme.html)

Class Theme
===========
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#theme){#theme}

Theme
=====
:::

Represents a Theme definition available in the current installation of
Drafts.

[](#example-find-and-assign-the-active-light-theme){#example-find-and-assign-the-active-light-theme}

### Example: Find and assign the active light theme

    let theme = Theme.find("builtIn", "dark");
    app.lightTheme = theme;
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Theme]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Identification Properties

-   [installURL](theme.html#installurl){.tsd-kind-icon}
-   [name](theme.html#name){.tsd-kind-icon}
-   [type](theme.html#type){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [find](theme.html#find){.tsd-kind-icon}
-   [getAll](theme.html#getall){.tsd-kind-icon}
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
    [Theme.d.ts:31](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Theme.d.ts#L31)

::: {.tsd-comment .tsd-typography}
::: {.lead}
URL which can be used to install this Theme in another installation of
Drafts. Useful for sharing and backups.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#name .tsd-anchor}

### name

::: {.tsd-signature .tsd-kind-icon}
name[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Theme.d.ts:25](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Theme.d.ts#L25)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The name of the theme definition.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#type .tsd-anchor}

### type

::: {.tsd-signature .tsd-kind-icon}
type[:]{.tsd-signature-symbol}
[themeType](../globals.html#themetype){.tsd-signature-type}
:::

-   Defined in
    [Theme.d.ts:19](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Theme.d.ts#L19)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The type (builtIn, custom, file) of the theme definition.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#find .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} find

-   find[(]{.tsd-signature-symbol}type[:
    ]{.tsd-signature-symbol}[themeType](../globals.html#themetype){.tsd-signature-type},
    name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Theme](theme.html){.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Theme.d.ts:41](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Theme.d.ts#L41)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Search for a theme definition matching the type and name passed and
    return it if found. Returns undefined if not found.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### type: [themeType](../globals.html#themetype){.tsd-signature-type}

    -   ##### name: [string]{.tsd-signature-type}

    #### Returns [Theme](theme.html){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-theme-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#getall .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} getAll

-   getAll[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Theme](theme.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Theme.d.ts:36](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Theme.d.ts#L36)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get list of all available themees.
    :::
    :::

    #### Returns [Theme](theme.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-theme .tsd-returns-title}
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
-   [Theme](theme.html){.tsd-kind-icon}
    -   [installURL](theme.html#installurl){.tsd-kind-icon}
    -   [name](theme.html#name){.tsd-kind-icon}
    -   [type](theme.html#type){.tsd-kind-icon}
    -   [find](theme.html#find){.tsd-kind-icon}
    -   [getAll](theme.html#getall){.tsd-kind-icon}

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
