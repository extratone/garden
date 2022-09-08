---
{"dg-publish":true,"permalink":"/snippets/shellscript/","dgHomeLink":true,"dgPassFrontmatter":false}
---

shellscript

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
-   [ShellScript](shellscript.html)

Class ShellScript
=================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#shellscript){#shellscript}

ShellScript
===========
:::

***macOS only**. Requires Drafts 19 or greater.*

ShellScript objects can be used to execute Unix shell scripts.

[](#bash-example){#bash-example}

### Bash Example

    // define text of bash script
    let script = `#!/bin/bash
    echo "Total arguments : $#"
    echo "1st Argument = $1"
    echo "2nd argument = $2"
    `;
    let runner = ShellScript.create(script);

    if (runner.execute(["1", "2"])) {
        alert("STDOUT: " + runner.standardOutput);
    }
    else {
        alert("STDERR: " + runner.standardError);
    }

[](#ruby-example){#ruby-example}

### Ruby Example

    let script = `#!/usr/bin/env ruby
    ARGV.each do |a|
      puts "Argument: #{a}"
    end
    `;
    let runner = ShellScript.create(script);

    if (runner.execute(["1", "2"])) {
        alert("STDOUT:\n" + runner.standardOutput);
    }
    else {
        alert("STDERR:\n" + runner.standardError);
    }

**Note:** When executed, scripts are saved to temporary files in the
Drafts\' script directory at
`~/Library/Application Scripts/com.agiletortoise.Drafts-OSX` and run.
Scripts should not be written to make assumptions about their location
in the file system (e.g. using relative paths). The first time a script
is executed, the user will be asked to grant permissions to the script
directory.
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [ShellScript]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](shellscript.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [standardError](shellscript.html#standarderror){.tsd-kind-icon}
-   [standardOutput](shellscript.html#standardoutput){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [execute](shellscript.html#execute){.tsd-kind-icon}
-   [create](shellscript.html#create){.tsd-kind-icon}
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

-   new ShellScript[(]{.tsd-signature-symbol}script[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[ShellScript](shellscript.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [ShellScript.d.ts:62](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ShellScript.d.ts#L62)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### script: [string]{.tsd-signature-type}

    #### Returns [ShellScript](shellscript.html){.tsd-signature-type} {#returns-shellscript .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#standarderror .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} standardError

::: {.tsd-signature .tsd-kind-icon}
standardError[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}[
\| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}
:::

-   Defined in
    [ShellScript.d.ts:51](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ShellScript.d.ts#L51)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Content sent to standard error during the execution of the script
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#standardoutput .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} standardOutput

::: {.tsd-signature .tsd-kind-icon}
standardOutput[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}[
\| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}
:::

-   Defined in
    [ShellScript.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ShellScript.d.ts#L56)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Content sent to standard output during the execution of the script
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

-   execute[(]{.tsd-signature-symbol}arguments[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [ShellScript.d.ts:74](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ShellScript.d.ts#L74)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Executes the shell script.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### arguments: [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        An array of string arguments to pass to the script. These will
        appear to the script as command line arguments would.
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}

    `true` if the script was executed without error, `false` if not.
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}script[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[ShellScript](shellscript.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [ShellScript.d.ts:62](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/ShellScript.d.ts#L62)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Convenience method to create a ShellScript object.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### script: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        A string containing the shell script. This should contain the
        appropriate \"she bang\" to trigger the appropriate scripting
        language/shell.
        :::

    #### Returns [ShellScript](shellscript.html){.tsd-signature-type} {#returns-shellscript-1 .tsd-returns-title}
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
-   [ShellScript](shellscript.html){.tsd-kind-icon}
    -   [constructor](shellscript.html#constructor){.tsd-kind-icon}
    -   [standardError](shellscript.html#standarderror){.tsd-kind-icon}
    -   [standardOutput](shellscript.html#standardoutput){.tsd-kind-icon}
    -   [execute](shellscript.html#execute){.tsd-kind-icon}
    -   [create](shellscript.html#create){.tsd-kind-icon}

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
