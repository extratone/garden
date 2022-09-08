---
{"dg-publish":true,"permalink":"/snippets/multimarkdown/","dgHomeLink":true,"dgPassFrontmatter":false}
---

multimarkdown

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
-   [MultiMarkdown](multimarkdown.html)

Class MultiMarkdown
===================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#multimarkdown){#multimarkdown}

MultiMarkdown
=============
:::

Drafts includes a full version of the MultiMarkdown 6 engine to render
Markdown text to HTML and other supported formats. For details on the
meaning of the various options, refer to [MultiMarkdown
documentation](https://github.com/fletcher/MultiMarkdown-6).

[](#example){#example}

### Example

    var inputString = "# Header\n\nMy **markdown** text";
    var mmd = MultiMarkdown.create();

    mmd.format = "html";
    mmd.criticMarkup = true;
    var outputString = mmd.render(inputString);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [MultiMarkdown]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](multimarkdown.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [completeDocument](multimarkdown.html#completedocument){.tsd-kind-icon}
-   [criticMarkup](multimarkdown.html#criticmarkup){.tsd-kind-icon}
-   [criticMarkupAccept](multimarkdown.html#criticmarkupaccept){.tsd-kind-icon}
-   [criticMarkupReject](multimarkdown.html#criticmarkupreject){.tsd-kind-icon}
-   [footnotesEnabled](multimarkdown.html#footnotesenabled){.tsd-kind-icon}
-   [format](multimarkdown.html#format){.tsd-kind-icon}
-   [markdownCompatibilityMode](multimarkdown.html#markdowncompatibilitymode){.tsd-kind-icon}
-   [noLabels](multimarkdown.html#nolabels){.tsd-kind-icon}
-   [noMetadata](multimarkdown.html#nometadata){.tsd-kind-icon}
-   [obfuscate](multimarkdown.html#obfuscate){.tsd-kind-icon}
-   [processHTML](multimarkdown.html#processhtml){.tsd-kind-icon}
-   [randomFootnotes](multimarkdown.html#randomfootnotes){.tsd-kind-icon}
-   [smartQuotesEnabled](multimarkdown.html#smartquotesenabled){.tsd-kind-icon}
-   [snippetOnly](multimarkdown.html#snippetonly){.tsd-kind-icon}
-   [transclude](multimarkdown.html#transclude){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [render](multimarkdown.html#render){.tsd-kind-icon}
-   [create](multimarkdown.html#create){.tsd-kind-icon}
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
    MultiMarkdown[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[MultiMarkdown](multimarkdown.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MultiMarkdown.d.ts:93](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L93)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [MultiMarkdown](multimarkdown.html){.tsd-signature-type} {#returns-multimarkdown .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#completedocument .tsd-anchor}

### completeDocument

::: {.tsd-signature .tsd-kind-icon}
completeDocument[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:42](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L42)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#criticmarkup .tsd-anchor}

### criticMarkup

::: {.tsd-signature .tsd-kind-icon}
criticMarkup[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:74](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L74)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#criticmarkupaccept .tsd-anchor}

### criticMarkupAccept

::: {.tsd-signature .tsd-kind-icon}
criticMarkupAccept[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:78](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L78)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#criticmarkupreject .tsd-anchor}

### criticMarkupReject

::: {.tsd-signature .tsd-kind-icon}
criticMarkupReject[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:82](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L82)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#footnotesenabled .tsd-anchor}

### footnotesEnabled

::: {.tsd-signature .tsd-kind-icon}
footnotesEnabled[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:54](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L54)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `true`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#format .tsd-anchor}

### format

::: {.tsd-signature .tsd-kind-icon}
format[:]{.tsd-signature-symbol} [\"html\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"epub\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"latex\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"beamer\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"memoir\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"odt\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"mmd\"]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:33](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L33)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Specify output format. Valid values are:

-   `html`: HTML. This is the default Markdown output.
-   `epub`: ePub
-   `latex`: LaTeX
-   `beamer`
-   `memoir`
-   `odt`: Open document format
-   `mmd`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#markdowncompatibilitymode .tsd-anchor}

### markdownCompatibilityMode

::: {.tsd-signature .tsd-kind-icon}
markdownCompatibilityMode[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:38](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L38)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#nolabels .tsd-anchor}

### noLabels

::: {.tsd-signature .tsd-kind-icon}
noLabels[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:58](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L58)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `true`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#nometadata .tsd-anchor}

### noMetadata

::: {.tsd-signature .tsd-kind-icon}
noMetadata[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:66](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L66)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#obfuscate .tsd-anchor}

### obfuscate

::: {.tsd-signature .tsd-kind-icon}
obfuscate[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:70](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L70)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#processhtml .tsd-anchor}

### processHTML

::: {.tsd-signature .tsd-kind-icon}
processHTML[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:62](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L62)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `true`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#randomfootnotes .tsd-anchor}

### randomFootnotes

::: {.tsd-signature .tsd-kind-icon}
randomFootnotes[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:86](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L86)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#smartquotesenabled .tsd-anchor}

### smartQuotesEnabled

::: {.tsd-signature .tsd-kind-icon}
smartQuotesEnabled[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L50)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `true`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#snippetonly .tsd-anchor}

### snippetOnly

::: {.tsd-signature .tsd-kind-icon}
snippetOnly[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:46](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L46)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#transclude .tsd-anchor}

### transclude

::: {.tsd-signature .tsd-kind-icon}
transclude[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [MultiMarkdown.d.ts:90](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L90)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to `false`
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#render .tsd-anchor}

### render

-   render[(]{.tsd-signature-symbol}markdownStr[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MultiMarkdown.d.ts:21](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L21)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Takes Markdown string passed and processes it with MultiMarkdown
    based on the properties and format selections on the object.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### markdownStr: [string]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type} {#returns-string .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[MultiMarkdown](multimarkdown.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MultiMarkdown.d.ts:93](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MultiMarkdown.d.ts#L93)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create object
    :::
    :::

    #### Returns [MultiMarkdown](multimarkdown.html){.tsd-signature-type} {#returns-multimarkdown-1 .tsd-returns-title}
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
-   [MultiMarkdown](multimarkdown.html){.tsd-kind-icon}
    -   [constructor](multimarkdown.html#constructor){.tsd-kind-icon}
    -   [completeDocument](multimarkdown.html#completedocument){.tsd-kind-icon}
    -   [criticMarkup](multimarkdown.html#criticmarkup){.tsd-kind-icon}
    -   [criticMarkupAccept](multimarkdown.html#criticmarkupaccept){.tsd-kind-icon}
    -   [criticMarkupReject](multimarkdown.html#criticmarkupreject){.tsd-kind-icon}
    -   [footnotesEnabled](multimarkdown.html#footnotesenabled){.tsd-kind-icon}
    -   [format](multimarkdown.html#format){.tsd-kind-icon}
    -   [markdownCompatibilityMode](multimarkdown.html#markdowncompatibilitymode){.tsd-kind-icon}
    -   [noLabels](multimarkdown.html#nolabels){.tsd-kind-icon}
    -   [noMetadata](multimarkdown.html#nometadata){.tsd-kind-icon}
    -   [obfuscate](multimarkdown.html#obfuscate){.tsd-kind-icon}
    -   [processHTML](multimarkdown.html#processhtml){.tsd-kind-icon}
    -   [randomFootnotes](multimarkdown.html#randomfootnotes){.tsd-kind-icon}
    -   [smartQuotesEnabled](multimarkdown.html#smartquotesenabled){.tsd-kind-icon}
    -   [snippetOnly](multimarkdown.html#snippetonly){.tsd-kind-icon}
    -   [transclude](multimarkdown.html#transclude){.tsd-kind-icon}
    -   [render](multimarkdown.html#render){.tsd-kind-icon}
    -   [create](multimarkdown.html#create){.tsd-kind-icon}

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
