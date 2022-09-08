---
{"dg-publish":true,"permalink":"/snippets/onedrive/","dgHomeLink":true,"dgPassFrontmatter":false}
---

onedrive

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
-   [OneDrive](onedrive.html)

Class OneDrive
==============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#onedrive){#onedrive}

OneDrive
========
:::

OneDrive objects can be used to work with files in a OneDrive account.

[](#example){#example}

### Example

    // create OneDrive object
    var drive = OneDrive.create();

    // setup variables
    var path = "/test/file.txt";
    var content = "text to place in file";

    // write to file on OneDrive
    var success = drive.write(path, content, false);

    if (success) { // write worked!
      var driveContent = drive.read(path);
      if (driveContent) { // read worked!
        if (driveContent == content) {
          alert("File contents match!");
        }
        else {
          console.log("File did not match");
          context.fail();
        }
      }
      else { // read failed, log error
        console.log(drive.lastError);
        context.fail();
      }
    }
    else { // write failed, log error
      console.log(drive.lastError);
      context.fail();
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [OneDrive]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](onedrive.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [lastError](onedrive.html#lasterror){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [read](onedrive.html#read){.tsd-kind-icon}
-   [write](onedrive.html#write){.tsd-kind-icon}
-   [create](onedrive.html#create){.tsd-kind-icon}
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

-   new OneDrive[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[OneDrive](onedrive.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [OneDrive.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OneDrive.d.ts#L64)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [OneDrive](onedrive.html){.tsd-signature-type} {#returns-onedrive .tsd-returns-title}
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
    [OneDrive.d.ts:45](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OneDrive.d.ts#L45)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function fails, this property will contain the last error as a
string message, otherwise it will be undefined.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#read .tsd-anchor}

### read

-   read[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [OneDrive.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OneDrive.d.ts#L50)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Reads the contents of the file at the path as a string. Returns
    undefined value if the file does not exist or could not be read.
    Paths should begin with a `/` and be relative to the root directory
    of your OneDrive.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type} {#returns-string .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#write .tsd-anchor}

### write

-   write[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, content[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, overwrite[?:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [OneDrive.d.ts:58](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OneDrive.d.ts#L58)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Write the contents of the file at the path. Returns true if
    successful, false if the file could not be written successfully.
    This will override existing files!
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Paths should begin with a `/` and be relative to the root
        directory of your OneDrive
        :::

    -   ##### content: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Text to place in the file
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} overwrite: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        If `false`, an existing file will not be overwritten
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[OneDrive](onedrive.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [OneDrive.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OneDrive.d.ts#L64)

    ::: {.tsd-comment .tsd-typography}
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional identifier for OneDrive account to use. This string is
        an arbitrary value, but we recommend using the email address you
        wish to associate with the script. Each unique identifier will
        be associated with its own
        [Credential](https://getdrafts.com/settings/credentials).
        :::

    #### Returns [OneDrive](onedrive.html){.tsd-signature-type} {#returns-onedrive-1 .tsd-returns-title}
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
-   [OneDrive](onedrive.html){.tsd-kind-icon}
    -   [constructor](onedrive.html#constructor){.tsd-kind-icon}
    -   [lastError](onedrive.html#lasterror){.tsd-kind-icon}
    -   [read](onedrive.html#read){.tsd-kind-icon}
    -   [write](onedrive.html#write){.tsd-kind-icon}
    -   [create](onedrive.html#create){.tsd-kind-icon}

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
