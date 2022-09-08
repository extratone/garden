---
{"dg-publish":true,"permalink":"/snippets/xmlrpcresponse/","dgHomeLink":true,"dgPassFrontmatter":false}
---

xmlrpcresponse

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
-   [XMLRPCResponse](xmlrpcresponse.html)

Class XMLRPCResponse
====================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#xmlrpcresponse){#xmlrpcresponse}

XMLRPCResponse
==============
:::

XMLRPCResponse objects are returned by calls to using XML-RPC
interfaces. For details on using XML-RPC, see [XMLRPC](xmlrpc.html)
object reference.
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [XMLRPCResponse]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [error](xmlrpcresponse.html#error){.tsd-kind-icon}
-   [faultCode](xmlrpcresponse.html#faultcode){.tsd-kind-icon}
-   [params](xmlrpcresponse.html#params){.tsd-kind-icon}
-   [statusCode](xmlrpcresponse.html#statuscode){.tsd-kind-icon}
-   [success](xmlrpcresponse.html#success){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#error .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} error

::: {.tsd-signature .tsd-kind-icon}
error[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [XML-RPC.d.ts:71](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/XML-RPC.d.ts#L71)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If an error occurred, a description of the type of error.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#faultcode .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} faultCode

::: {.tsd-signature .tsd-kind-icon}
faultCode[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [XML-RPC.d.ts:66](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/XML-RPC.d.ts#L66)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If the XML-RPC interface returned an error, the error code will be here.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#params .tsd-anchor}

### params

::: {.tsd-signature .tsd-kind-icon}
params[:]{.tsd-signature-symbol}
[any]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [XML-RPC.d.ts:61](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/XML-RPC.d.ts#L61)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The array of return parameters provided by with the XML-RPC response.
Contents of this array will vary with the XML-RPC API being used.
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
    [XML-RPC.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/XML-RPC.d.ts#L56)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The HTTP status code (like 200, 301, etc.) returned. This will be 200 if
communication with the XML-RPC endpoint was successful, even if a fault
occurred processing the request. Be sure to use the `success` property
and `faultCode` to check for errors.
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
    [XML-RPC.d.ts:51](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/XML-RPC.d.ts#L51)

::: {.tsd-comment .tsd-typography}
::: {.lead}
whether the request was completed successfully. This value will be
`true` if both the HTTP status code is 200 and no fault code was
returned from the API.
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
-   [XMLRPCResponse](xmlrpcresponse.html){.tsd-kind-icon}
    -   [error](xmlrpcresponse.html#error){.tsd-kind-icon}
    -   [faultCode](xmlrpcresponse.html#faultcode){.tsd-kind-icon}
    -   [params](xmlrpcresponse.html#params){.tsd-kind-icon}
    -   [statusCode](xmlrpcresponse.html#statuscode){.tsd-kind-icon}
    -   [success](xmlrpcresponse.html#success){.tsd-kind-icon}

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
