---
{"dg-publish":true,"permalink":"/snippets/share/","dgHomeLink":true,"dgPassFrontmatter":false}
---

share

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
-   [Share](share.html)

Class Share
===========
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#share){#share}

Share
=====
:::

Methods to share via system share sheet.

[](#example){#example}

### Example

    let s = "My text to share"

    let didShare = Share.shareAsText(s);
    let didShare = Share.shareAsURL("http://getdrafts.com/");
    let didShare = Share.shareAsFile("My-File.txt", s);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Share]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Methods

-   [shareAsFile](share.html#shareasfile){.tsd-kind-icon}
-   [shareAsText](share.html#shareastext){.tsd-kind-icon}
-   [shareAsURL](share.html#shareasurl){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#shareasfile .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} shareAsFile

-   shareAsFile[(]{.tsd-signature-symbol}filename[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, text[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Share.d.ts:31](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Share.d.ts#L31)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open system share sheet to share the content as a file, with the
    specified file name (with e). Returns `true` if share was completed
    by user amd `false` if input was invalid or user cancelled share.
    Drafts will create a temporary file for the purposes of the share
    and send it to the share sheet. The temporary file will be deleted
    after. Useful, for example, to create a text file and share to Mail,
    and it will be shared as an attachment to the email
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### filename: [string]{.tsd-signature-type}

    -   ##### text: [string]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#shareastext .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} shareAsText

-   shareAsText[(]{.tsd-signature-symbol}text[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Share.d.ts:20](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Share.d.ts#L20)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open system share sheet to share the string provided as text.
    Returns `true` if share was completed by user, `false` if input was
    invalid or user cancelled the share.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### text: [string]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#shareasurl .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} shareAsURL

-   shareAsURL[(]{.tsd-signature-symbol}url[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Share.d.ts:26](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Share.d.ts#L26)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open system share sheet to share the url provided as a URL object.
    Returns `true` if share was completed by user and `false` if input
    was invalid or user cancelled share.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### url: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        should be a complete and valid URL
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-2 .tsd-returns-title}
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
-   [Share](share.html){.tsd-kind-icon}
    -   [shareAsFile](share.html#shareasfile){.tsd-kind-icon}
    -   [shareAsText](share.html#shareastext){.tsd-kind-icon}
    -   [shareAsURL](share.html#shareasurl){.tsd-kind-icon}

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
