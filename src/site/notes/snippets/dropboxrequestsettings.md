---
{"dg-publish":true,"permalink":"/snippets/dropboxrequestsettings/","dgHomeLink":true,"dgPassFrontmatter":false}
---

dropboxrequestsettings

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
-   [DropboxRequestSettings](dropboxrequestsettings.html)

Interface DropboxRequestSettings
================================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [DropboxRequestSettings]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [data](dropboxrequestsettings.html#data){.tsd-kind-icon}
-   [dropbox-api-args](dropboxrequestsettings.html#dropbox_api_args){.tsd-kind-icon}
-   [headers](dropboxrequestsettings.html#headers){.tsd-kind-icon}
-   [method](dropboxrequestsettings.html#method){.tsd-kind-icon}
-   [parameters](dropboxrequestsettings.html#parameters){.tsd-kind-icon}
-   [url](dropboxrequestsettings.html#url){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-interface}
[]{#data .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} data

::: {.tsd-signature .tsd-kind-icon}
data[:]{.tsd-signature-symbol} [{}]{.tsd-signature-symbol}
:::

-   Defined in
    [Dropbox.d.ts:19](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L19)

::: {.tsd-comment .tsd-typography}
::: {.lead}
An object containing data to be encoded into the HTTP body of the
request.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-interface}
[]{#dropbox_api_args .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} dropbox-api-args

::: {.tsd-signature .tsd-kind-icon}
dropbox-api-args[:]{.tsd-signature-symbol} [{}]{.tsd-signature-symbol}
:::

-   Defined in
    [Dropbox.d.ts:21](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L21)

::: {.tsd-comment .tsd-typography}
::: {.lead}
An object containing the parameters to encode in the `dropbox-api-args`
header, per API documentation. Drafts will take care of properly ASCII
escaping values. Required only for `contentUploadRequest` and
`contentDownloadRequest` functions.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-interface}
[]{#headers .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} headers

::: {.tsd-signature .tsd-kind-icon}
headers[:]{.tsd-signature-symbol} [{}]{.tsd-signature-symbol}
:::

-   Defined in
    [Dropbox.d.ts:15](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L15)

::: {.tsd-comment .tsd-typography}
::: {.lead}
An object contain key-values to be added as custom headers in the
request.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-interface}
[]{#method .tsd-anchor}

### method

::: {.tsd-signature .tsd-kind-icon}
method[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Dropbox.d.ts:11](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L11)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The HTTP method, like \"GET\", \"POST\", etc.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-interface}
[]{#parameters .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} parameters

::: {.tsd-signature .tsd-kind-icon}
parameters[:]{.tsd-signature-symbol} [{}]{.tsd-signature-symbol}
:::

-   Defined in
    [Dropbox.d.ts:17](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L17)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Query parameters to merge with the url. Query parameters can also be
part of the original url value.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-interface}
[]{#url .tsd-anchor}

### url

::: {.tsd-signature .tsd-kind-icon}
url[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Dropbox.d.ts:7](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L7)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The full URL to the RPC endpoint in the [Dropbox
API](https://www.dropbox.com/developers/documentation/http/documentation).
RPC endpoint are typically on the `api.dropboxapi.com` domain.
:::
:::
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
-   [DropboxRequestSettings](dropboxrequestsettings.html){.tsd-kind-icon}
    -   [data](dropboxrequestsettings.html#data){.tsd-kind-icon}
    -   [dropbox-api-args](dropboxrequestsettings.html#dropbox_api_args){.tsd-kind-icon}
    -   [headers](dropboxrequestsettings.html#headers){.tsd-kind-icon}
    -   [method](dropboxrequestsettings.html#method){.tsd-kind-icon}
    -   [parameters](dropboxrequestsettings.html#parameters){.tsd-kind-icon}
    -   [url](dropboxrequestsettings.html#url){.tsd-kind-icon}

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
