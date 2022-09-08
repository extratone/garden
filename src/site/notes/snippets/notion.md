---
{"dg-publish":true,"permalink":"/snippets/notion/","dgHomeLink":true,"dgPassFrontmatter":false}
---

notion

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
-   [Notion](notion.html)

Class Notion
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#notion){#notion}

Notion
======
:::

Script integration with [Notion](https://www.notion.so/). This object
handles OAuth authentication and request signing. The entire [Notion
REST API](https://developers.notion.com) can be used with the `request`
method.

[](#example){#example}

### Example

    // list pages which have been shared with the Drafts integration
    // API Docs: https://developers.notion.com/reference/post-search
    let endpoint = "https://api.notion.com/v1/search"

    let notion = Notion.create();
    let result = notion.request({
        "url": endpoint,
        "method": "POST",
        "data": {
            "filter": {
                "value": "page",
                "property": "object"
            }
        }
    });

    // result has JSON payload
    // with page properties
    if (result.statusCode == 200) {
        alert(`Notion Pages Loaded:

    ${result.responseText}`)
    }
    else {
        alert(`Notion Error: ${result.statusCode}

    ${notion.lastError}`);
        context.fail();
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Notion]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](notion.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [lastError](notion.html#lasterror){.tsd-kind-icon}
-   [lastResponse](notion.html#lastresponse){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [request](notion.html#request){.tsd-kind-icon}
-   [create](notion.html#create){.tsd-kind-icon}
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

-   new Notion[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Notion](notion.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Notion.d.ts:74](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Notion.d.ts#L74)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [Notion](notion.html){.tsd-signature-type} {#returns-notion .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lasterror .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} lastError

::: {.tsd-signature .tsd-kind-icon}
lastError[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Notion.d.ts:49](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Notion.d.ts#L49)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function fails, this property will contain the last error as a
string message, otherwise it will be `undefined`.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lastresponse .tsd-anchor}

### lastResponse

::: {.tsd-signature .tsd-kind-icon}
lastResponse[:]{.tsd-signature-symbol} [any]{.tsd-signature-type}
:::

-   Defined in
    [Notion.d.ts:44](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Notion.d.ts#L44)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function succeeds, this property will contain the last response
returned by Notion. The JSON returned by Notion will be parsed to an
object and placed in this property. Refer to [Notion API
documentation](https://developers.notion.com) for details on the
contents of this object based on call made.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#request .tsd-anchor}

### request

-   request[(]{.tsd-signature-symbol}settings[:
    ]{.tsd-signature-symbol}[{ ]{.tsd-signature-symbol}data[?:
    ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[;
    ]{.tsd-signature-symbol}headers[?:
    ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[;
    ]{.tsd-signature-symbol}method[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[;
    ]{.tsd-signature-symbol}parameters[?:
    ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[;
    ]{.tsd-signature-symbol}url[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[
    }]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[HTTPResponse](httpresponse.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Notion.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Notion.d.ts#L57)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Execute a request against the Notion API. For successful requests,
    the HTTPResponse object will contain an object or array or objects
    decoded from the JSON returned by Notion as appropriate to the
    request made. Refer to Notion\'s API documentation for details about
    the expected parameters and responses. Drafts will handle wrapping
    the request in the appropriate OAuth authentication flow.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### settings: [{ ]{.tsd-signature-symbol}data[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}headers[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}method[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[; ]{.tsd-signature-symbol}parameters[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}url[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[ }]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        an object configuring the request.
        :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} data[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            A JavaScript object containing data to be encoded into the
            HTTP body of the request. Refer to API documentation for
            appropriate information to include.
            :::
            :::

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} headers[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            An object contain key-values to be added as custom headers
            in the request. There is no need to provide authorization
            headers, Drafts will add those. Drafts will automatically
            include required authentication and versioning headers.
            :::
            :::

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### method[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            The HTTP method, like \"GET\", \"POST\", etc.
            :::
            :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} parameters[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            An object containing key-values to be added to the request
            as URL parameters.
            :::
            :::

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### url[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            The full URL to the endpoint in the [Notion REST
            API](hhttps://developers.notion.com.).
            :::
            :::

    #### Returns [HTTPResponse](httpresponse.html){.tsd-signature-type} {#returns-httpresponse .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Notion](notion.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Notion.d.ts:74](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Notion.d.ts#L74)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new Notion object.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional string value used to identify a Notion account.
        Typically this can be omitted if you only work with one Notion
        account in Drafts. Each unique identifier used for Notion
        accounts will share credentials - across both action steps and
        scripts.
        :::

    #### Returns [Notion](notion.html){.tsd-signature-type} {#returns-notion-1 .tsd-returns-title}
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
-   [Notion](notion.html){.tsd-kind-icon}
    -   [constructor](notion.html#constructor){.tsd-kind-icon}
    -   [lastError](notion.html#lasterror){.tsd-kind-icon}
    -   [lastResponse](notion.html#lastresponse){.tsd-kind-icon}
    -   [request](notion.html#request){.tsd-kind-icon}
    -   [create](notion.html#create){.tsd-kind-icon}

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
