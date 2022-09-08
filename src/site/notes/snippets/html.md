---
{"dg-publish":true,"permalink":"/snippets/html/","dgHomeLink":true,"dgPassFrontmatter":false}
---

html

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
-   [HTML](html.html)

Class HTML
==========
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#html){#html}

HTML
====
:::

Helper methods to escape and unescape HTML entities in a string.

*Added: R15*

[](#examples){#examples}

### Examples

    let s = "<One> & Two";
    let escaped = HTML.escape(s); // "&#x3C;One&#x3E &#x26; Two"
    let unescaped = HTML.unescape(encoded); // "<One> & Two"
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [HTML]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Methods

-   [escape](html.html#escape){.tsd-kind-icon}
-   [unescape](html.html#unescape){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#escape .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} escape

-   escape[(]{.tsd-signature-symbol}string[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [HTML.d.ts:21](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTML.d.ts#L21)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Escape HTML entities in a string to be HTML safe.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### string: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        the string to escape
        :::

    #### Returns [string]{.tsd-signature-type} {#returns-string .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#unescape .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} unescape

-   unescape[(]{.tsd-signature-symbol}string[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [HTML.d.ts:27](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTML.d.ts#L27)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Unescape HTML entities in a string.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### string: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        the string to unescape
        :::

    #### Returns [string]{.tsd-signature-type} {#returns-string-1 .tsd-returns-title}
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
-   [HTML](html.html){.tsd-kind-icon}
    -   [escape](html.html#escape){.tsd-kind-icon}
    -   [unescape](html.html#unescape){.tsd-kind-icon}

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
