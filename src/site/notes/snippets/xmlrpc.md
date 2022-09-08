---
{"dg-publish":true,"permalink":"/snippets/xmlrpc/","dgHomeLink":true,"dgPassFrontmatter":false}
---

xmlrpc

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
-   [XMLRPC](xmlrpc.html)

Class XMLRPC
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#xmlrpc){#xmlrpc}

XMLRPC
======
:::

The XMLRPC object is a convenience method to provide an easy way to
[XML-RPC](http://xmlrpc.scripting.com/) web services. The request
function takes care of converting native Javascript objects and values
to the XML parameters required for the XML-RPC interface, and converts
the XML responses returned to Javascript objects.

It will also return faults parsed to error messages in the response if
necessary.

This object is suitable for communication with a number of popular
XML-RPC interfaces, including the [MetaWeblog
API](http://xmlrpc.scripting.com/metaWeblogApi.html). WordPress also
offers its own XML-RPC interface, which can be used via this object, or
the convenience wrapper `WordPress` object.

[](#example-xml-rpc-call){#example-xml-rpc-call}

### Example: XML-RPC call

    // DEMO of XML-RPC
    // Calls example method on http://xml-rpc.net/index.html

    let url = "http://www.cookcomputing.com/xmlrpcsamples/RPC2.ashx";
    let methodName = "examples.getStateName";
    let params = [20];

    let response = XMLRPC.request(url, methodName, params);

    if (response.success) {
        alert(JSON.stringify(response.params));
    }
    else {
        alert("Fault: " + response.faultCode + ", " + response.error);
        context.fail();
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [XMLRPC]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Methods

-   [request](xmlrpc.html#request){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#request .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} request

-   request[(]{.tsd-signature-symbol}url[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, methodName[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, params[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[XMLRPCResponse](xmlrpcresponse.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [XML-RPC.d.ts:39](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/XML-RPC.d.ts#L39)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Make an XML-RPC request.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### url: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The full URL of the XML-RPC host endpoint being called.
        :::

    -   ##### methodName: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Name of the method to call. Supported values are specific to the
        services provided by the host.
        :::

    -   ##### params: [any]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        The parameters to pass to the request. This should be an array
        of values, in the proper order, as specified by the
        documentation of the host being called. This array will be
        encoded into XML-RPC parameters in XML format by the method -
        only raw javascript values should be provided.
        :::

    #### Returns [XMLRPCResponse](xmlrpcresponse.html){.tsd-signature-type} {#returns-xmlrpcresponse .tsd-returns-title}
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
-   [XMLRPC](xmlrpc.html){.tsd-kind-icon}
    -   [request](xmlrpc.html#request){.tsd-kind-icon}

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
