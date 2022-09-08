---
{"dg-publish":true,"permalink":"/snippets/context/","dgHomeLink":true,"dgPassFrontmatter":false}
---

context

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
-   [Context](context.html)

Class Context
=============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#context){#context}

Context
=======
:::

A single global \"context\" object is available to scripts to control
flow of the currently running action.

It is important to understand that `cancel()` and `fail()` will not
immediately stop script, just stop any further action steps from being
performed.

[](#example-control-flow){#example-control-flow}

### Example: Control Flow

    // test for logical condition before continuing
    if (!validationCondition) {
      context.fail();
    }
    // code below will still run.

[](#example-retreive-values){#example-retreive-values}

### Example: Retreive values

    // if a "Run Workflow" step preceded this script, lets look for a result
    var response = context.callbackResponses[0];
    if (response) {
      // Workflow returns one "result" parameter, other apps may use other values.
      var result = response["result"];
      if (result) {
        // so something with the result
      }
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Context]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [appleScriptResponses](context.html#applescriptresponses){.tsd-kind-icon}
-   [callbackResponses](context.html#callbackresponses){.tsd-kind-icon}
-   [previewValues](context.html#previewvalues){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [addSuccessParameter](context.html#addsuccessparameter){.tsd-kind-icon}
-   [cancel](context.html#cancel){.tsd-kind-icon}
-   [fail](context.html#fail){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#applescriptresponses .tsd-anchor}

### appleScriptResponses

::: {.tsd-signature .tsd-kind-icon}
appleScriptResponses[:]{.tsd-signature-symbol}
[{}]{.tsd-signature-symbol}
:::

-   Defined in
    [Context.d.ts:42](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Context.d.ts#L42)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If AppleScripts run using the AppleScript object return values, they
will be converted to JavaScript object and stored in this array. See
[AppleScript
docs](https://docs.getdrafts.com/docs/automation/applescript) for
details.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[any]{.tsd-signature-type}
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#callbackresponses .tsd-anchor}

### callbackResponses

::: {.tsd-signature .tsd-kind-icon}
callbackResponses[:]{.tsd-signature-symbol} [{}]{.tsd-signature-symbol}
:::

-   Defined in
    [Context.d.ts:37](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Context.d.ts#L37)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If [Callback
URL](https://docs.getdrafts.com/docs/actions/steps/advanced#callback-url)
or [Run
Shortcut](https://docs.getdrafts.com/docs/actions/steps/advanced#run-shortcut)
action steps using the \"Wait for response\" option have been run in
steps before the script step in an action, and the target app returned
to Drafts using an x-success callback, this object will contain an array
of objects with the parsed query parameters included in those responses,
in the order they were received.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[any]{.tsd-signature-type}
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#previewvalues .tsd-anchor}

### previewValues

::: {.tsd-signature .tsd-kind-icon}
previewValues[:]{.tsd-signature-symbol} [{
]{.tsd-signature-symbol}string[:
]{.tsd-signature-symbol}[any]{.tsd-signature-type}[
}]{.tsd-signature-symbol}
:::

-   Defined in
    [Context.d.ts:47](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Context.d.ts#L47)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If [HTML Preview](https://docs.getdrafts.com/docs/actions/html-forms)
makes calls to `Drafts.send(key, value)` those values are stored in this
object by `key`.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### string[: ]{.tsd-signature-symbol}[any]{.tsd-signature-type}
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addsuccessparameter .tsd-anchor}

### addSuccessParameter

-   addSuccessParameter[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, value[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Context.d.ts:71](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Context.d.ts#L71)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Used only when calling a Drafts action from another app via
    x-callback-url with a `/runAction` URL. Any parameters set via this
    method will be included as query args when calling the provided
    `x-success` parameter. As an example, the below:
    :::

        context.addSuccessParameter("a", "1");
        context.addSuccessParameter("b", "2");

    Would result in the parameters `?a=1&b=2` being added to the
    `x-success` callback.
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The name for the parameter
        :::

    -   ##### value: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        A string value for the parameter. Do *not* URL encode this
        value, it will be encoded when added to the callback URL.
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#cancel .tsd-anchor}

### cancel

-   cancel[(]{.tsd-signature-symbol}message[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Context.d.ts:52](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Context.d.ts#L52)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Tell the context to cancel the action at the end of the script
    execution. If called, at the end of the script the action will be
    stopped. No subsequent action steps in the action will run, and the
    action still stop silently - no notification banners, sounds, etc.
    If a message is included it will be added to the action log to
    explain the cancellation.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### message: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#fail .tsd-anchor}

### fail

-   fail[(]{.tsd-signature-symbol}message[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Context.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Context.d.ts#L57)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Tell the context to fail the current action. In effect this is the
    same as `cancel()` but an error notification will be shown. If a
    message is included it will be added to the action log to explain
    the cancellation.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### message: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-2 .tsd-returns-title}
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
-   [Context](context.html){.tsd-kind-icon}
    -   [appleScriptResponses](context.html#applescriptresponses){.tsd-kind-icon}
    -   [callbackResponses](context.html#callbackresponses){.tsd-kind-icon}
    -   [previewValues](context.html#previewvalues){.tsd-kind-icon}
    -   [addSuccessParameter](context.html#addsuccessparameter){.tsd-kind-icon}
    -   [cancel](context.html#cancel){.tsd-kind-icon}
    -   [fail](context.html#fail){.tsd-kind-icon}

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
