---
{"dg-publish":true,"permalink":"/snippets/applescript/","dgHomeLink":true,"dgPassFrontmatter":false}
---

applescript

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
-   [AppleScript](applescript.html)

Class AppleScript
=================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#applescript){#applescript}

AppleScript
===========
:::

***macOS only**. Requires Drafts 19 or greater.*

AppleScript objects can be used to execute AppleScripts. It is highly
recommended AppleScripts be developed and tested in Apple\'s Script
Editor or similar AppleScript editor, and loaded in Drafts when
completed.

[](#example){#example}

### Example

    // create a local file in App documents
    let method = "execute";
    let script = `on execute(bodyHTML)
        tell application "Safari"
            activate
        end tell
        return "Yeah!"
    end execute`;

    let html = draft.processTemplate("");

    let runner = AppleScript.create(script);
    if (runner.execute(method, [html])) {
        // the AppleScript ran without error
        // if the script returned a result, it's available...
        alert(runner.lastResult);
    }
    else {
        alert(runner.lastError);
    }

**Note:** When executed, AppleScripts are saved to temporary files in
the Drafts\' script directory at
`~/Library/Application Scripts/com.agiletortoise.Drafts-OSX` and run.
The first time a script is executed, the user will be asked to grant
permissions to the script directory.
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [AppleScript]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](applescript.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [lastError](applescript.html#lasterror){.tsd-kind-icon}
-   [lastResult](applescript.html#lastresult){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [execute](applescript.html#execute){.tsd-kind-icon}
-   [create](applescript.html#create){.tsd-kind-icon}
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

-   new AppleScript[(]{.tsd-signature-symbol}script[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[AppleScript](applescript.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [AppleScript.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/AppleScript.d.ts#L50)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### script: [string]{.tsd-signature-type}

    #### Returns [AppleScript](applescript.html){.tsd-signature-type} {#returns-applescript .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lasterror .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} lastError

::: {.tsd-signature .tsd-kind-icon}
lastError[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}
:::

-   Defined in
    [AppleScript.d.ts:39](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/AppleScript.d.ts#L39)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function fails, this property will contain the last error as a
string message, otherwise it will be `undefined`.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lastresult .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} lastResult

::: {.tsd-signature .tsd-kind-icon}
lastResult[:]{.tsd-signature-symbol} [object]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}
:::

-   Defined in
    [AppleScript.d.ts:44](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/AppleScript.d.ts#L44)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a the AppleScript subroutine called returns a value and it can be
converted to a JavaScript object, it will be stored here. Most basic
data types (string, date, numbers), as well as list and records
containing those data types, can be returned.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#execute .tsd-anchor}

### execute

-   execute[(]{.tsd-signature-symbol}subroutine[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, arguments[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [AppleScript.d.ts:63](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/AppleScript.d.ts#L63)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Compiles and executes the AppleScript code, calling the subroutine
    passed with the arguments.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### subroutine: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The name of a subroutine in the AppleScript to call.
        [Subroutines](http://www.macosxautomation.com/applescript/sbrt/)
        are defined using `on subroutineName()` syntax in the
        AppleScript.
        :::

    -   ##### arguments: [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        An array of arguments to pass to the subroutine. Most basic
        Javascript data types, and objects and arrays of those data
        types, can be passed and will be translated to the proper
        AppleScript types.
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}

    `true` if the AppleScript was compiled and executed without error,
    `false` if not. If `false`, the `lastError` property will contain
    details regarding the error.
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}script[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[AppleScript](applescript.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [AppleScript.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/AppleScript.d.ts#L50)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Convenience method to create an AppleScript object.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### script: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        A string containing the AppleScript code. This code will be
        compiled and executed when the `execute` function is called.
        :::

    #### Returns [AppleScript](applescript.html){.tsd-signature-type} {#returns-applescript-1 .tsd-returns-title}
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
-   [AppleScript](applescript.html){.tsd-kind-icon}
    -   [constructor](applescript.html#constructor){.tsd-kind-icon}
    -   [lastError](applescript.html#lasterror){.tsd-kind-icon}
    -   [lastResult](applescript.html#lastresult){.tsd-kind-icon}
    -   [execute](applescript.html#execute){.tsd-kind-icon}
    -   [create](applescript.html#create){.tsd-kind-icon}

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
