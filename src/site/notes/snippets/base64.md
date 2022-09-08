---
{"dg-publish":true,"permalink":"/snippets/base64/","dgHomeLink":true,"dgPassFrontmatter":false}
---

base64

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
-   [Base64](base64.html)

Class Base64
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#base64){#base64}

Base64
======
:::

Helper methods to encode and decode
[Base64](https://en.wikipedia.org/wiki/Base64) strings.

[](#examples){#examples}

### Examples

    let s = "My String";
    let encoded = Base64.encode(s);
    let decoded = Base64.decode(encoded);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Base64]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Methods

-   [decode](base64.html#decode){.tsd-kind-icon}
-   [encode](base64.html#encode){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#decode .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} decode

-   decode[(]{.tsd-signature-symbol}data[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Base64.d.ts:25](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Base64.d.ts#L25)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Base64 decode a string.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### data: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        the string to decode
        :::

    #### Returns [string]{.tsd-signature-type} {#returns-string .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#encode .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} encode

-   encode[(]{.tsd-signature-symbol}data[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Base64.d.ts:19](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Base64.d.ts#L19)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Base64 encode a string.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### data: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        the string to encode
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
-   [Base64](base64.html){.tsd-kind-icon}
    -   [decode](base64.html#decode){.tsd-kind-icon}
    -   [encode](base64.html#encode){.tsd-kind-icon}

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
