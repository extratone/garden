---
{"dg-publish":true,"permalink":"/snippets/httpresponse/","dgHomeLink":true,"dgPassFrontmatter":false}
---

httpresponse

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
-   [HTTPResponse](httpresponse.html)

Class HTTPResponse
==================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#httpresponse){#httpresponse}

HTTPResponse
============
:::

HTTPResponse objects are returned by calls to HTTP methods. For usage
details, see [HTTP](http.html) object.
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [HTTPResponse]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [error](httpresponse.html#error){.tsd-kind-icon}
-   [headers](httpresponse.html#headers){.tsd-kind-icon}
-   [otherData](httpresponse.html#otherdata){.tsd-kind-icon}
-   [responseData](httpresponse.html#responsedata){.tsd-kind-icon}
-   [responseText](httpresponse.html#responsetext){.tsd-kind-icon}
-   [statusCode](httpresponse.html#statuscode){.tsd-kind-icon}
-   [success](httpresponse.html#success){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#error .tsd-anchor}

### error

::: {.tsd-signature .tsd-kind-icon}
error[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}
:::

-   Defined in
    [HTTP.d.ts:111](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTTP.d.ts#L111)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If an error occurred, a description of the type of error.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#headers .tsd-anchor}

### headers

::: {.tsd-signature .tsd-kind-icon}
headers[:]{.tsd-signature-symbol} [object]{.tsd-signature-type}
:::

-   Defined in
    [HTTP.d.ts:101](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTTP.d.ts#L101)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Key-value dictionary containing any HTTP header information returned
with the response. Useful for access cookie headers, etc.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#otherdata .tsd-anchor}

### otherData

::: {.tsd-signature .tsd-kind-icon}
otherData[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}
:::

-   Defined in
    [HTTP.d.ts:106](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTTP.d.ts#L106)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Some responses return additional data that is placed in this field.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#responsedata .tsd-anchor}

### responseData

::: {.tsd-signature .tsd-kind-icon}
responseData[:]{.tsd-signature-symbol} [any]{.tsd-signature-type}
:::

-   Defined in
    [HTTP.d.ts:91](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTTP.d.ts#L91)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The raw data returned. Typically an object or array of objects, but
exact content varies by server response.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#responsetext .tsd-anchor}

### responseText

::: {.tsd-signature .tsd-kind-icon}
responseText[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [HTTP.d.ts:96](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTTP.d.ts#L96)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The data returned as a string format.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#statuscode .tsd-anchor}

### statusCode

::: {.tsd-signature .tsd-kind-icon}
statusCode[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [HTTP.d.ts:86](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTTP.d.ts#L86)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The HTTP status code (like 200, 301, etc.) returned.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#success .tsd-anchor}

### success

::: {.tsd-signature .tsd-kind-icon}
success[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [HTTP.d.ts:81](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/HTTP.d.ts#L81)

::: {.tsd-comment .tsd-typography}
::: {.lead}
true/false for whether the request was completed successfully.
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
-   [HTTPResponse](httpresponse.html){.tsd-kind-icon}
    -   [error](httpresponse.html#error){.tsd-kind-icon}
    -   [headers](httpresponse.html#headers){.tsd-kind-icon}
    -   [otherData](httpresponse.html#otherdata){.tsd-kind-icon}
    -   [responseData](httpresponse.html#responsedata){.tsd-kind-icon}
    -   [responseText](httpresponse.html#responsetext){.tsd-kind-icon}
    -   [statusCode](httpresponse.html#statuscode){.tsd-kind-icon}
    -   [success](httpresponse.html#success){.tsd-kind-icon}

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
