---
{"dg-publish":true,"permalink":"/snippets/medium/","dgHomeLink":true,"dgPassFrontmatter":false}
---

medium

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
-   [Medium](medium.html)

Class Medium
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#medium){#medium}

Medium
======
:::

Script integration with [Medium.com](http://medium.com/). This object
handles OAuth authentication and request signing. The entire [Medium
REST API](https://github.com/Medium/medium-api-docs) can be used with
the `request` method, and convenience methods are provided for common
API endpoints to get user information, list publications and post.

If an API calls fails, typically the result will be an `undefined`
value, and the `lastError` property will contains error detail
information for troubleshooting.
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Medium]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](medium.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [lastError](medium.html#lasterror){.tsd-kind-icon}
-   [lastResponse](medium.html#lastresponse){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [createPost](medium.html#createpost){.tsd-kind-icon}
-   [getUser](medium.html#getuser){.tsd-kind-icon}
-   [listPublications](medium.html#listpublications){.tsd-kind-icon}
-   [request](medium.html#request){.tsd-kind-icon}
-   [create](medium.html#create){.tsd-kind-icon}
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

-   new Medium[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Medium](medium.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Medium.d.ts:59](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Medium.d.ts#L59)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [Medium](medium.html){.tsd-signature-type} {#returns-medium .tsd-returns-title}
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
    [Medium.d.ts:18](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Medium.d.ts#L18)

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
    [Medium.d.ts:13](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Medium.d.ts#L13)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function success, this property will contain the last response
returned by Medium. The JSON returned by Medium will be parsed to an
object and placed in this property. Refer to [Medium API
documentation](https://github.com/Medium/medium-api-docs) for details on
the contents of this object based on call made.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createpost .tsd-anchor}

### createPost

-   createPost[(]{.tsd-signature-symbol}userId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Medium.d.ts:34](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Medium.d.ts#L34)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a post in the user\'s Medium stories. See [API
    docs](https://github.com/Medium/medium-api-docs) for details on what
    should be included in the options.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### userId: [string]{.tsd-signature-type}

    -   ##### options: [object]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        :::

    #### Returns [object]{.tsd-signature-type} {#returns-object .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getuser .tsd-anchor}

### getUser

-   getUser[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Medium.d.ts:24](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Medium.d.ts#L24)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get User information for current authenticated user. This will
    include the `id` property needed for other calls.
    :::
    :::

    #### Returns [object]{.tsd-signature-type} {#returns-object-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#listpublications .tsd-anchor}

### listPublications

-   listPublications[(]{.tsd-signature-symbol}userId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Medium.d.ts:28](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Medium.d.ts#L28)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get list of publications for current authenticated user.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### userId: [string]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-object-2 .tsd-returns-title}
:::

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
        [Medium.d.ts:42](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Medium.d.ts#L42)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Execute a request against the Medium API. For successful requests,
    the HTTPResponse object will contain an object or array or objects
    decoded from the JSON returned by Medium as appropriate to the
    request made. Refer to Medium API documentation for details about
    the expected parameters and responses. Drafts will handle wrapping
    the request in the appropriate OAuth authentication flow.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### settings: [{ ]{.tsd-signature-symbol}data[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}headers[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}method[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[; ]{.tsd-signature-symbol}parameters[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}url[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[ }]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        an object configuring the request.
        :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} data[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            A JavaScript object containing data to be encoded into the
            HTTP body of the request.
            :::
            :::

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} headers[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            An object contain key-values to be added as custom headers
            in the request. There is no need to provide authorization
            headers, Drafts will add those.
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
            The full URL to the endpoint in the [Medium REST
            API](https://github.com/Medium/medium-api-docs).
            :::
            :::

    #### Returns [HTTPResponse](httpresponse.html){.tsd-signature-type} {#returns-httpresponse .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Medium.d.ts:59](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Medium.d.ts#L59)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new Medium object.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional string value used to identify a Medium account.
        Typically this can be omitted if you only work with one Medium
        account in Drafts. Each unique identifier used for Medium
        accounts will share credentials - across both action steps and
        scripts.
        :::

    #### Returns [any]{.tsd-signature-type} {#returns-any .tsd-returns-title}
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
-   [Medium](medium.html){.tsd-kind-icon}
    -   [constructor](medium.html#constructor){.tsd-kind-icon}
    -   [lastError](medium.html#lasterror){.tsd-kind-icon}
    -   [lastResponse](medium.html#lastresponse){.tsd-kind-icon}
    -   [createPost](medium.html#createpost){.tsd-kind-icon}
    -   [getUser](medium.html#getuser){.tsd-kind-icon}
    -   [listPublications](medium.html#listpublications){.tsd-kind-icon}
    -   [request](medium.html#request){.tsd-kind-icon}
    -   [create](medium.html#create){.tsd-kind-icon}

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
