---
{"dg-publish":true,"permalink":"/snippets/twitter/","dgHomeLink":true,"dgPassFrontmatter":false}
---

twitter

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
-   [Twitter](twitter.html)

Class Twitter
=============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#twitter){#twitter}

Twitter
=======
:::

Script integration with Twitter. The `updateStatus` method is a
convenience method for posting a tweet, but the entire [Twitter
API](https://developer.twitter.com/en/docs/api-reference-index) can be
used with the request method, which handles OAuth authentication and
authorization.

[](#example){#example}

### Example

    // create twitter object
    var twitter = Twitter.create();
    // post tweet
    var success = twitter.updateStatus("My tweet content!");

    if success {
      console.log(twitter.lastResponse);
    }
    else {
      console.log(twitter.lastError);
      context.fail();
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Twitter]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](twitter.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [request](twitter.html#request){.tsd-kind-icon}
-   [updateStatus](twitter.html#updatestatus){.tsd-kind-icon}
-   [create](twitter.html#create){.tsd-kind-icon}
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

-   new Twitter[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Twitter](twitter.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Twitter.d.ts:49](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Twitter.d.ts#L49)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [Twitter](twitter.html){.tsd-signature-type} {#returns-twitter .tsd-returns-title}
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
        [Twitter.d.ts:38](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Twitter.d.ts#L38)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Execute a request against the Twitter API. For successful requests,
    the \[\[\[HTTPResponse\]\] object will contain an object or array or
    objects decoded from the JSON returned by Twitter as appropriate to
    the request made. Refer to Twitter's API documentation for details
    about the expected parameters and responses. Drafts will handle
    wrapping the request in the appropriate OAuth authentication flow.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### settings: [{ ]{.tsd-signature-symbol}data[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}headers[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}method[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[; ]{.tsd-signature-symbol}parameters[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}url[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[ }]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        an object with the following properties:

        -   url \[string, required\]: The full URL to the endpoint in
            the [Twitter
            API](https://developer.twitter.com/en/docs/api-reference-index).
        -   method \[string, required\]: The HTTP method, like \"GET\",
            \"POST\", etc.
        -   headers \[object, optional\]: An object contain key-values
            to be added as custom headers in the request. There is no
            need to provide authorization headers, Drafts will add
            those.
        -   parameters \[object, optional\]: An object containing
            key-values to be added to the request as URL parameters.
        -   data \[object, optional\]: An object containing data to be
            encoded into the HTTP body of the request.
        :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} data[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} headers[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### method[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} parameters[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### url[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

    #### Returns [HTTPResponse](httpresponse.html){.tsd-signature-type} {#returns-httpresponse .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#updatestatus .tsd-anchor}

### updateStatus

-   updateStatus[(]{.tsd-signature-symbol}content[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Twitter.d.ts:27](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Twitter.d.ts#L27)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Post a status update (tweet) to Twitter. Returns `true` if
    successful, `false` if not. After success the `lastResponse` object
    can be used to inspect response and get details such as the ID of
    the tweet created. Refer to [Twitter API POST /status/update
    documentation](https://developer.twitter.com/en/docs/tweets/post-and-engage/api-reference/post-statuses-update)
    for response details.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### content: [string]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Twitter](twitter.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Twitter.d.ts:49](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Twitter.d.ts#L49)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new Twitter object. Identifier is a optional string value
    used to identify a Twitter account. Typically this can be omitted if
    you only work with one Twitter account in Drafts. Each unique
    identifier used for Twitter accounts will share credentials - across
    both action steps and scripts.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

    #### Returns [Twitter](twitter.html){.tsd-signature-type} {#returns-twitter-1 .tsd-returns-title}
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
-   [Twitter](twitter.html){.tsd-kind-icon}
    -   [constructor](twitter.html#constructor){.tsd-kind-icon}
    -   [request](twitter.html#request){.tsd-kind-icon}
    -   [updateStatus](twitter.html#updatestatus){.tsd-kind-icon}
    -   [create](twitter.html#create){.tsd-kind-icon}

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
