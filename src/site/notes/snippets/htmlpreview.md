---
{"dg-publish":true,"permalink":"/snippets/htmlpreview/","dgHomeLink":true,"dgPassFrontmatter":false}
---

htmlpreview

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
-   [HTMLPreview](htmlpreview.html)

Class HTMLPreview
=================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#htmlpreview){#htmlpreview}

HTMLPreview
===========
:::

Display of HTML Preview window, the same as the HTMLPreview action step.
Returns true if user closed preview with the \"Continue\" button, false
if the user cancelled.

[](#example){#example}

### Example

    let html = "<html><body>My Document</body></html>"

    let preview = HTMLPreview.create();
    if (preview.show(html)) {
      // continue button was pressed
    }
    else {
      // cancel button was pressed
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [HTMLPreview]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](htmlpreview.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [hideInterface](htmlpreview.html#hideinterface){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [show](htmlpreview.html#show){.tsd-kind-icon}
-   [create](htmlpreview.html#create){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Constructors
------------

::: {.section .tsd-panel .tsd-member .tsd-kind-constructor .tsd-parent-kind-class}
[]{#constructor .tsd-anchor}

### constructor

-   new
    HTMLPreview[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[HTMLPreview](htmlpreview.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [HTMLPreview.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTMLPreview.d.ts#L35)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [HTMLPreview](htmlpreview.html){.tsd-signature-type} {#returns-htmlpreview .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#hideinterface .tsd-anchor}

### hideInterface

::: {.tsd-signature .tsd-kind-icon}
hideInterface[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [HTMLPreview.d.ts:24](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTMLPreview.d.ts#L24)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Hides the toolbars and `Cancel` / `Continue` buttons in the preview
window. For use only when combined with JavaScript flow control in the
HTML preview. See [docs]() for details.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#show .tsd-anchor}

### show

-   show[(]{.tsd-signature-symbol}html[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [HTMLPreview.d.ts:30](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTMLPreview.d.ts#L30)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open HTML Preview window displaying the HTML string passed.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### html: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The HTML content to display. Should be complete HTML document.
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[HTMLPreview](htmlpreview.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [HTMLPreview.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTMLPreview.d.ts#L35)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [HTMLPreview](htmlpreview.html){.tsd-signature-type} {#returns-htmlpreview-1 .tsd-returns-title}
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
-   [HTMLPreview](htmlpreview.html){.tsd-kind-icon}
    -   [constructor](htmlpreview.html#constructor){.tsd-kind-icon}
    -   [hideInterface](htmlpreview.html#hideinterface){.tsd-kind-icon}
    -   [show](htmlpreview.html#show){.tsd-kind-icon}
    -   [create](htmlpreview.html#create){.tsd-kind-icon}

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
