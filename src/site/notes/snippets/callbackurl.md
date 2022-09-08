---
{"dg-publish":true,"permalink":"/snippets/callbackurl/","dgHomeLink":true,"dgPassFrontmatter":false}
---

callbackurl

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
-   [CallbackURL](callbackurl.html)

Class CallbackURL
=================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#callbackurl){#callbackurl}

CallbackURL
===========
:::

CallbackURL objects can be used to open x-callback-url requests and wait
for a response from the target app.

**NOTE**: If you want to open a URL in Safari or another app and do not
need a response or x-callback-url support, use the `app.openURL(url)`
method on the App object.

[](#example){#example}

### Example

    // Open callback URL for each line in a draft
    // Setup base Fantastical URL, with no parameters
    const baseURL = "fantastical2://x-callback-url/parse/";

    // split draft and loop over lines
    var lines = draft.content.split("\n");
    for (var line of lines) {
        // create and configure callback object
        var cb = CallbackURL.create();
        cb.baseURL = baseURL;
        cb.addParameter("sentence", line);
        // open and wait for result
        var success = cb.open();
        if (success) {
            console.log("Event created");
        }
        else { // something went wrong or was cancelled
              console.log(cb.status);
              if (cb.status == "cancelled") {
                context.cancel();
            }
            else {
                context.fail();
            }
        }
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [CallbackURL]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](callbackurl.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [baseURL](callbackurl.html#baseurl){.tsd-kind-icon}
-   [callbackResponse](callbackurl.html#callbackresponse){.tsd-kind-icon}
-   [parameters](callbackurl.html#parameters){.tsd-kind-icon}
-   [status](callbackurl.html#status){.tsd-kind-icon}
-   [url](callbackurl.html#url){.tsd-kind-icon}
-   [waitForResponse](callbackurl.html#waitforresponse){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [addParameter](callbackurl.html#addparameter){.tsd-kind-icon}
-   [open](callbackurl.html#open){.tsd-kind-icon}
-   [create](callbackurl.html#create){.tsd-kind-icon}
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
    CallbackURL[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[CallbackURL](callbackurl.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [CallbackURL.d.ts:90](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L90)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [CallbackURL](callbackurl.html){.tsd-signature-type} {#returns-callbackurl .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#baseurl .tsd-anchor}

### baseURL

::: {.tsd-signature .tsd-kind-icon}
baseURL[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [CallbackURL.d.ts:43](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L43)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The baseURL of the request. This should include the x-callback-url base
URL and action, typically something like
`app-scheme://x-callback-url/actionName`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#callbackresponse .tsd-anchor}

### callbackResponse

::: {.tsd-signature .tsd-kind-icon}
callbackResponse[:]{.tsd-signature-symbol} [{}]{.tsd-signature-symbol}
:::

-   Defined in
    [CallbackURL.d.ts:74](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L74)

::: {.tsd-comment .tsd-typography}
::: {.lead}
An object contain and URL query parameters returned by the target app
along with it's callback response. For example, if the target app called
x-success with the query parameters `result=MyTestText`,
callbackResponse would contain `{"result": "MyTestText"}`.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[any]{.tsd-signature-type}
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#parameters .tsd-anchor}

### parameters

::: {.tsd-signature .tsd-kind-icon}
parameters[:]{.tsd-signature-symbol} [{}]{.tsd-signature-symbol}
:::

-   Defined in
    [CallbackURL.d.ts:58](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L58)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Object containing string keys and values to be appended to the base url
as query parameters. Values should not be pre-encoded, but will be
encoded and added to the base URL automatically. Do not include
x-callback parameters (`x-success`, `x-error`, `x-cancel`) as these will
be generated by Drafts.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[any]{.tsd-signature-type}
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#status .tsd-anchor}

### status

::: {.tsd-signature .tsd-kind-icon}
status[:]{.tsd-signature-symbol} [\"created\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"success\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"cancelled\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"error\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"timeout\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"invalid\"]{.tsd-signature-type}
:::

-   Defined in
    [CallbackURL.d.ts:69](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L69)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The current status of the callback. Used to check outcome after open is
called. Possible values:

-   created: open has not yet been called.
-   success: x-success callback was received from target app.
-   cancelled: x-cancel callback was received from target app.
-   error: x-error callback was received from target app.
-   timeout: Waiting for the response timed out without receiving a
    callback URL from the target app.
-   invalid: The URL was invalid and could not be opened.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#url .tsd-anchor}

### url

::: {.tsd-signature .tsd-kind-icon}
url[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [CallbackURL.d.ts:48](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L48)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The current URL. This is provided as a debugging property, and will
output the URL including the baseURL property with any configured
parameters added. This property will differ from the actual URL opened
when calling `open()` in that it will not contain the `x-success`,
`x-error` and `x-cancel` parameters which are added dynamically at the
time `open()` is called.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#waitforresponse .tsd-anchor}

### waitForResponse

::: {.tsd-signature .tsd-kind-icon}
waitForResponse[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [CallbackURL.d.ts:53](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L53)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If true, the script will pause and wait for the `x-success`, `x-error`
or `x-cancel` response from the app being targeted by the URL. If false,
execution of the script/action will continue immediately and no
response/results will be available.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addparameter .tsd-anchor}

### addParameter

-   addParameter[(]{.tsd-signature-symbol}key[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, value[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [CallbackURL.d.ts:85](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L85)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a query parameter for the outgoing URL. FIXME: can the value be
    anything?
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### key: [string]{.tsd-signature-type}

    -   ##### value: [any]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#open .tsd-anchor}

### open

-   open[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [CallbackURL.d.ts:79](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L79)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Opens the URL with associated parameters, and waits for a callback
    response. Returns true if an x-success response was received from
    the target app, otherwise false. If false, use the \"status\"
    property to determine the type of failure.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[CallbackURL](callbackurl.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [CallbackURL.d.ts:90](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/CallbackURL.d.ts#L90)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new CallbackURL object.
    :::
    :::

    #### Returns [CallbackURL](callbackurl.html){.tsd-signature-type} {#returns-callbackurl-1 .tsd-returns-title}
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
-   [CallbackURL](callbackurl.html){.tsd-kind-icon}
    -   [constructor](callbackurl.html#constructor){.tsd-kind-icon}
    -   [baseURL](callbackurl.html#baseurl){.tsd-kind-icon}
    -   [callbackResponse](callbackurl.html#callbackresponse){.tsd-kind-icon}
    -   [parameters](callbackurl.html#parameters){.tsd-kind-icon}
    -   [status](callbackurl.html#status){.tsd-kind-icon}
    -   [url](callbackurl.html#url){.tsd-kind-icon}
    -   [waitForResponse](callbackurl.html#waitforresponse){.tsd-kind-icon}
    -   [addParameter](callbackurl.html#addparameter){.tsd-kind-icon}
    -   [open](callbackurl.html#open){.tsd-kind-icon}
    -   [create](callbackurl.html#create){.tsd-kind-icon}

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
