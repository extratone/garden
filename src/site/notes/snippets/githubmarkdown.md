---
{"dg-publish":true,"permalink":"/snippets/githubmarkdown/","dgHomeLink":true,"dgPassFrontmatter":false}
---

githubmarkdown

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
-   [GitHubMarkdown](githubmarkdown.html)

Class GitHubMarkdown
====================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#githubmarkdown){#githubmarkdown}

GitHubMarkdown
==============
:::

Drafts includes Discount-based, GitHub flavored Markdown parser based on
[GHMarkdownParser](https://github.com/OliverLetterer/GHMarkdownParser).
For details on the meaning of the various options, refer to [Markdown
documentation](https://getdrafts.com/settings/markdown).

[](#example){#example}

### Example

    var inputString = "# Header\n\nMy **markdown** text";
    var md = GitHubMarkdown.create();

    var outputString = md.render(inputString);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [GitHubMarkdown]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](githubmarkdown.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [autoLinks](githubmarkdown.html#autolinks){.tsd-kind-icon}
-   [noImages](githubmarkdown.html#noimages){.tsd-kind-icon}
-   [noLinks](githubmarkdown.html#nolinks){.tsd-kind-icon}
-   [removeHTMLTags](githubmarkdown.html#removehtmltags){.tsd-kind-icon}
-   [safeLinks](githubmarkdown.html#safelinks){.tsd-kind-icon}
-   [smartQuotesEnabled](githubmarkdown.html#smartquotesenabled){.tsd-kind-icon}
-   [strict](githubmarkdown.html#strict){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [render](githubmarkdown.html#render){.tsd-kind-icon}
-   [create](githubmarkdown.html#create){.tsd-kind-icon}
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
    GitHubMarkdown[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[GitHubMarkdown](githubmarkdown.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GitHubMarkdown.d.ts:53](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L53)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [GitHubMarkdown](githubmarkdown.html){.tsd-signature-type} {#returns-githubmarkdown .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#autolinks .tsd-anchor}

### autoLinks

::: {.tsd-signature .tsd-kind-icon}
autoLinks[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [GitHubMarkdown.d.ts:40](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L40)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to false
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#noimages .tsd-anchor}

### noImages

::: {.tsd-signature .tsd-kind-icon}
noImages[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [GitHubMarkdown.d.ts:28](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L28)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to true
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#nolinks .tsd-anchor}

### noLinks

::: {.tsd-signature .tsd-kind-icon}
noLinks[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [GitHubMarkdown.d.ts:32](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L32)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to true
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#removehtmltags .tsd-anchor}

### removeHTMLTags

::: {.tsd-signature .tsd-kind-icon}
removeHTMLTags[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [GitHubMarkdown.d.ts:48](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L48)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to false
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#safelinks .tsd-anchor}

### safeLinks

::: {.tsd-signature .tsd-kind-icon}
safeLinks[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [GitHubMarkdown.d.ts:36](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L36)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to true
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
    [GitHubMarkdown.d.ts:24](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L24)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to true
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#strict .tsd-anchor}

### strict

::: {.tsd-signature .tsd-kind-icon}
strict[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [GitHubMarkdown.d.ts:44](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L44)

::: {.tsd-comment .tsd-typography}
::: {.lead}
defaults to false
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
        [GitHubMarkdown.d.ts:19](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L19)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Takes Markdown string passed and processes it with GitHub Markdown
    parser based on the property selections on the object.
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
    ]{.tsd-signature-symbol}[GitHubMarkdown](githubmarkdown.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GitHubMarkdown.d.ts:53](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GitHubMarkdown.d.ts#L53)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    create a new object.
    :::
    :::

    #### Returns [GitHubMarkdown](githubmarkdown.html){.tsd-signature-type} {#returns-githubmarkdown-1 .tsd-returns-title}
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
-   [GitHubMarkdown](githubmarkdown.html){.tsd-kind-icon}
    -   [constructor](githubmarkdown.html#constructor){.tsd-kind-icon}
    -   [autoLinks](githubmarkdown.html#autolinks){.tsd-kind-icon}
    -   [noImages](githubmarkdown.html#noimages){.tsd-kind-icon}
    -   [noLinks](githubmarkdown.html#nolinks){.tsd-kind-icon}
    -   [removeHTMLTags](githubmarkdown.html#removehtmltags){.tsd-kind-icon}
    -   [safeLinks](githubmarkdown.html#safelinks){.tsd-kind-icon}
    -   [smartQuotesEnabled](githubmarkdown.html#smartquotesenabled){.tsd-kind-icon}
    -   [strict](githubmarkdown.html#strict){.tsd-kind-icon}
    -   [render](githubmarkdown.html#render){.tsd-kind-icon}
    -   [create](githubmarkdown.html#create){.tsd-kind-icon}

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
