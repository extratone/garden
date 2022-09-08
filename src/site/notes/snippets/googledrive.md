---
{"dg-publish":true,"permalink":"/snippets/googledrive/","dgHomeLink":true,"dgPassFrontmatter":false}
---

googledrive

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
-   [GoogleDrive](googledrive.html)

Class GoogleDrive
=================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#googledrive){#googledrive}

GoogleDrive
===========
:::

GoogleDrive objects can be used to work with files in Google Drive
accounts.

[](#example){#example}

### Example

    // create GoogleDrive object
    var drive = GoogleDrive.create();

    // setup variables
    var fileName = "MyTestFile";
    var parent = ""; // root of drive
    var content = "text to place in file";

    // write to file on GoogleDrive
    var success = drive.write(fileName, parent, content);

    if (success) { // write worked!
      var driveContent = drive.read(fileName, parent);
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

-   [GoogleDrive]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](googledrive.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [lastError](googledrive.html#lasterror){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [read](googledrive.html#read){.tsd-kind-icon}
-   [write](googledrive.html#write){.tsd-kind-icon}
-   [create](googledrive.html#create){.tsd-kind-icon}
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

-   new GoogleDrive[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[GoogleDrive](googledrive.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleDrive.d.ts:67](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleDrive.d.ts#L67)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [GoogleDrive](googledrive.html){.tsd-signature-type} {#returns-googledrive .tsd-returns-title}
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
    [GoogleDrive.d.ts:46](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleDrive.d.ts#L46)

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
[]{#read .tsd-anchor}

### read

-   read[(]{.tsd-signature-symbol}fileName[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, parent[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleDrive.d.ts:53](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleDrive.d.ts#L53)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Reads the contents of the file at the with the file name, in the
    parent folder, as a string. Returns `undefined` value if the file
    does not exist or could not be read.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### fileName: [string]{.tsd-signature-type}

    -   ##### parent: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Name of folder in the root of the Google Drive, or `""` for
        root. FIXME: optional?
        :::

    #### Returns [string]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-string-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#write .tsd-anchor}

### write

-   write[(]{.tsd-signature-symbol}fileName[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, parent[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, content[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleDrive.d.ts:61](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleDrive.d.ts#L61)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Write the contents of the file at the path. Returns true if
    successful, false if the file could not be written successfully.
    This will override existing files!
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### fileName: [string]{.tsd-signature-type}

    -   ##### parent: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Name of folder in the root of the Google Drive, or `""` for
        root.
        :::

    -   ##### content: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Text to write to file.
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[GoogleDrive](googledrive.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleDrive.d.ts:67](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleDrive.d.ts#L67)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new GoogleDrive object.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        used to identify a GoogleDrive account. Typically this can be
        omitted if you only work with one GoogleDrive account in Drafts.
        :::

    #### Returns [GoogleDrive](googledrive.html){.tsd-signature-type} {#returns-googledrive-1 .tsd-returns-title}
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
-   [GoogleDrive](googledrive.html){.tsd-kind-icon}
    -   [constructor](googledrive.html#constructor){.tsd-kind-icon}
    -   [lastError](googledrive.html#lasterror){.tsd-kind-icon}
    -   [read](googledrive.html#read){.tsd-kind-icon}
    -   [write](googledrive.html#write){.tsd-kind-icon}
    -   [create](googledrive.html#create){.tsd-kind-icon}

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
