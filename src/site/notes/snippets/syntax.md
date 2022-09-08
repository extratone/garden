---
{"dg-publish":true,"permalink":"/snippets/syntax/","dgHomeLink":true,"dgPassFrontmatter":false}
---

syntax

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
-   [Syntax](syntax.html)

Class Syntax
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#syntax){#syntax}

Syntax
======
:::

Represents a Syntax definition available in the current installation of
Drafts.

[](#example-find-and-assign-a-syntax){#example-find-and-assign-a-syntax}

### Example: Find and Assign a Syntax

    let syntax = Syntax.find("builtIn", "Markdown");
    draft.syntax = syntax;
    draft.update();
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Syntax]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Identification Properties

-   [installURL](syntax.html#installurl){.tsd-kind-icon}
-   [name](syntax.html#name){.tsd-kind-icon}
-   [type](syntax.html#type){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [find](syntax.html#find){.tsd-kind-icon}
-   [getAll](syntax.html#getall){.tsd-kind-icon}
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
    [Syntax.d.ts:32](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Syntax.d.ts#L32)

::: {.tsd-comment .tsd-typography}
::: {.lead}
URL which can be used to install this Syntax in another installation of
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
    [Syntax.d.ts:26](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Syntax.d.ts#L26)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The name of the syntax definition.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#type .tsd-anchor}

### type

::: {.tsd-signature .tsd-kind-icon}
type[:]{.tsd-signature-symbol}
[syntaxType](../globals.html#syntaxtype){.tsd-signature-type}
:::

-   Defined in
    [Syntax.d.ts:20](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Syntax.d.ts#L20)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The type (builtIn, custom, file) of the syntax definition.
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
    ]{.tsd-signature-symbol}[syntaxType](../globals.html#syntaxtype){.tsd-signature-type},
    name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Syntax](syntax.html){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Syntax.d.ts:42](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Syntax.d.ts#L42)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Search for a syntax definition matching the type and name passed and
    return it if found. Returns undefined if not found.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### type: [syntaxType](../globals.html#syntaxtype){.tsd-signature-type}

    -   ##### name: [string]{.tsd-signature-type}

    #### Returns [Syntax](syntax.html){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-syntax-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#getall .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} getAll

-   getAll[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Syntax](syntax.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Syntax.d.ts:37](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Syntax.d.ts#L37)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get list of all available syntaxes.
    :::
    :::

    #### Returns [Syntax](syntax.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-syntax .tsd-returns-title}
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
-   [Syntax](syntax.html){.tsd-kind-icon}
    -   [installURL](syntax.html#installurl){.tsd-kind-icon}
    -   [name](syntax.html#name){.tsd-kind-icon}
    -   [type](syntax.html#type){.tsd-kind-icon}
    -   [find](syntax.html#find){.tsd-kind-icon}
    -   [getAll](syntax.html#getall){.tsd-kind-icon}

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
