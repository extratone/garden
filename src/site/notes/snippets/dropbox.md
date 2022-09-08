---
{"dg-publish":true,"permalink":"/snippets/dropbox/","dgHomeLink":true,"dgPassFrontmatter":false}
---

dropbox

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
-   [Dropbox](dropbox.html)

Class Dropbox
=============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#dropbox){#dropbox}

Dropbox
=======
:::

Dropbox objects can be used to work with files in a
[Dropbox](http://dropbopx.com) account. The `read` and `write` methods
are simple wrappers for uploading and reading content of files on
Dropbox.

For advanced uses, the `rpcRequest`, `contentUploadRequest` and
`contentDownloadRequest` methods enable direct use of any Dropbox API
2.0 endpoints. These methods are an advanced feature which return raw
results from the Dropbox API and may require advanced understanding of
the API to process the results. They do enable full access to the API,
however, which enabled things like querying files, listing folder
contents, uploading to Paper, etc. For details on availalbe methods, see
[Dropbox API
documentation](https://www.dropbox.com/developers/documentation/http/overview).
In the case of all of these methods Drafts takes care of the OAuth
request signing and authentication process when necessary.

[](#example){#example}

### Example

    // create Dropbox object
    var db = Dropbox.create();

    // setup variables
    var path = "/test/file.txt";
    var content = "text to place in file";

    // write to file on Dropbox
    var success = db.write(path, content, "add", true);

    if (success) { // write worked!
      var dbContent = db.read(path);
      if (dbContent) { // read worked!
        if (dbContent == content) {
         alert("File contents match!");
        }
        else {
          console.log("File did not match");
          context.fail();
        }
      }
      else { // read failed, log error
        console.log(db.lastError);
        context.fail();
      }
    }
    else { // write failed, log error
      console.log(db.lastError);
      context.fail();
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Dropbox]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](dropbox.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [lastError](dropbox.html#lasterror){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [contentDownloadRequest](dropbox.html#contentdownloadrequest){.tsd-kind-icon}
-   [contentUploadRequest](dropbox.html#contentuploadrequest){.tsd-kind-icon}
-   [read](dropbox.html#read){.tsd-kind-icon}
-   [rpcRequest](dropbox.html#rpcrequest){.tsd-kind-icon}
-   [write](dropbox.html#write){.tsd-kind-icon}
-   [create](dropbox.html#create){.tsd-kind-icon}
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

-   new Dropbox[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Dropbox](dropbox.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Dropbox.d.ts:109](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L109)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [Dropbox](dropbox.html){.tsd-signature-type} {#returns-dropbox .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lasterror .tsd-anchor}

### lastError

::: {.tsd-signature .tsd-kind-icon}
lastError[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}
:::

-   Defined in
    [Dropbox.d.ts:70](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L70)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function fails, this property will contain the last error as a
string message, otherwise it will be `undefined`.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#contentdownloadrequest .tsd-anchor}

### contentDownloadRequest

-   contentDownloadRequest[(]{.tsd-signature-symbol}settings[:
    ]{.tsd-signature-symbol}[DropboxRequestSettings](../interfaces/dropboxrequestsettings.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[HTTPResponse](httpresponse.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Dropbox.d.ts:103](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L103)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Execute a request against the Dropbox API for an [endpoint of
    Content Download
    type](https://www.dropbox.com/developers/documentation/http/documentation#formats).
    For successful requests, the HTTPResponse object will contain an raw
    data in the `responseData` property and, if the data can be
    converted to a string value, the text version in the `responseText`
    property. The HTTPResponse `otherData` property will contain a
    Javascript object decoded from the JSON returned in the
    `Dropbox-API-Result` header. Refer to Dropbox\'s API documentation
    for details about the expected parameters and responses. Drafts will
    handle wrapping the request in the appropriate OAuth authentication
    flow.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### settings: [DropboxRequestSettings](../interfaces/dropboxrequestsettings.html){.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Object containing options for the request.
        :::

    #### Returns [HTTPResponse](httpresponse.html){.tsd-signature-type} {#returns-httpresponse .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#contentuploadrequest .tsd-anchor}

### contentUploadRequest

-   contentUploadRequest[(]{.tsd-signature-symbol}settings[:
    ]{.tsd-signature-symbol}[DropboxRequestSettings](../interfaces/dropboxrequestsettings.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[HTTPResponse](httpresponse.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Dropbox.d.ts:97](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L97)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Execute a request against the Dropbox API for an [endpoint of
    Content Upload
    type](https://www.dropbox.com/developers/documentation/http/documentation#formats).
    For successful requests, the HTTPResponse object will contain an
    object or array or objects decoded from the JSON returned by Dropbox
    as appropriate to the request made. Refer to Dropbox\'s API
    documentation for details about the expected parameters and
    responses. Drafts will handle wrapping the request in the
    appropriate OAuth authentication flow.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### settings: [DropboxRequestSettings](../interfaces/dropboxrequestsettings.html){.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Object containing options for the request.
        :::

    #### Returns [HTTPResponse](httpresponse.html){.tsd-signature-type} {#returns-httpresponse-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#read .tsd-anchor}

### read

-   read[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Dropbox.d.ts:76](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L76)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Reads the contents of the file at the with the file name, in the
    parent folder, as a string. Returns `undefined` value if the file
    does not exist or could not be read.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Path related to root of Dropbox folder.
        :::

    #### Returns [string]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-string-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#rpcrequest .tsd-anchor}

### rpcRequest

-   rpcRequest[(]{.tsd-signature-symbol}settings[:
    ]{.tsd-signature-symbol}[DropboxRequestSettings](../interfaces/dropboxrequestsettings.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[HTTPResponse](httpresponse.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Dropbox.d.ts:91](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L91)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Execute a request against the Dropbox API for an [endpoint of RPC
    type](https://www.dropbox.com/developers/documentation/http/documentation#formats).
    For successful requests, the HTTPResponse object will contain an
    object or array or objects decoded from the JSON returned by Dropbox
    as appropriate to the request made. Refer to Dropbox\'s API
    documentation for details about the expected parameters and
    responses. Drafts will handle wrapping the request in the
    appropriate OAuth authentication flow.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### settings: [DropboxRequestSettings](../interfaces/dropboxrequestsettings.html){.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Object containing options for the request.
        :::

    #### Returns [HTTPResponse](httpresponse.html){.tsd-signature-type} {#returns-httpresponse-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#write .tsd-anchor}

### write

-   write[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, content[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, mode[:
    ]{.tsd-signature-symbol}[dropboxMode](../globals.html#dropboxmode){.tsd-signature-type},
    autorename[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Dropbox.d.ts:85](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L85)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Write the contents of the file at the path. Returns true if
    successful, false if the file could not be written successfully.
    This will override existing files!
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Path related to root of Dropbox folder.
        :::

    -   ##### content: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Text to write to file.
        :::

    -   ##### mode: [dropboxMode](../globals.html#dropboxmode){.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Either \"add\" or \"overwrite\" to determine if the write method
        should overwrite an existing file at the path if it exists.
        :::

    -   ##### autorename: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Dropbox](dropbox.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Dropbox.d.ts:109](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Dropbox.d.ts#L109)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new Dropbox object.
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        used to identify a Dropbox account. Typically this can be
        omitted if you only work with one Dropbox account in Drafts.
        :::

    #### Returns [Dropbox](dropbox.html){.tsd-signature-type} {#returns-dropbox-1 .tsd-returns-title}
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
-   [Dropbox](dropbox.html){.tsd-kind-icon}
    -   [constructor](dropbox.html#constructor){.tsd-kind-icon}
    -   [lastError](dropbox.html#lasterror){.tsd-kind-icon}
    -   [contentDownloadRequest](dropbox.html#contentdownloadrequest){.tsd-kind-icon}
    -   [contentUploadRequest](dropbox.html#contentuploadrequest){.tsd-kind-icon}
    -   [read](dropbox.html#read){.tsd-kind-icon}
    -   [rpcRequest](dropbox.html#rpcrequest){.tsd-kind-icon}
    -   [write](dropbox.html#write){.tsd-kind-icon}
    -   [create](dropbox.html#create){.tsd-kind-icon}

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
