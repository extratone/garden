---
{"dg-publish":true,"permalink":"/snippets/filemanager/","dgHomeLink":true,"dgPassFrontmatter":false}
---

filemanager

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
-   [FileManager](filemanager.html)

Class FileManager
=================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#filemanager){#filemanager}

FileManager
===========
:::

FileManager objects can be used to read from or write to files in either
the local Drafts app Documents directory, or iCloud Drive (inside the
`Drafts` folder).Note that local files are not visible on iOS, and are
only available for reading and writing via scripting.

[](#example){#example}

### Example

    // create a local file in App documents
    let fmLocal = FileManager.createLocal(); // Local file in app container
    let success = fmLocal.writeString("/ScriptedFile.txt", "This is the file  * content");

    // read from file in iCloud
    let fmCloud = FileManager.createCloud(); // iCloud
    let content = fmCloud.readString("/Test Folder/Test.txt")

    // create a directory, and move a file to it
    fmCloud.createDirectory("My Folder", "/");
    fmCloud.moveItem("/TestFile.txt", "/My Folder/TestFile.txt", false);

    // create file manager using a Bookmark
    let bookmark = Bookmark.findOrCreate("My-Folder");
    let fm = FileManager.createForBookmark(bookmark);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [FileManager]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [basePath](filemanager.html#basepath){.tsd-kind-icon}
-   [baseURL](filemanager.html#baseurl){.tsd-kind-icon}
-   [lastError](filemanager.html#lasterror){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Attribute Methods

-   [getCreationDate](filemanager.html#getcreationdate){.tsd-kind-icon}
-   [getModificationDate](filemanager.html#getmodificationdate){.tsd-kind-icon}
-   [getTags](filemanager.html#gettags){.tsd-kind-icon}
-   [setCreationDate](filemanager.html#setcreationdate){.tsd-kind-icon}
-   [setModificationDate](filemanager.html#setmodificationdate){.tsd-kind-icon}
-   [setTags](filemanager.html#settags){.tsd-kind-icon}

### Constructors Methods

-   [create](filemanager.html#create){.tsd-kind-icon}
-   [createCloud](filemanager.html#createcloud){.tsd-kind-icon}
-   [createForBookmark](filemanager.html#createforbookmark){.tsd-kind-icon}
-   [createLocal](filemanager.html#createlocal){.tsd-kind-icon}

### Other Methods

-   [copyItem](filemanager.html#copyitem){.tsd-kind-icon}
-   [createDirectory](filemanager.html#createdirectory){.tsd-kind-icon}
-   [exists](filemanager.html#exists){.tsd-kind-icon}
-   [listContents](filemanager.html#listcontents){.tsd-kind-icon}
-   [moveItem](filemanager.html#moveitem){.tsd-kind-icon}
-   [readJSON](filemanager.html#readjson){.tsd-kind-icon}
-   [readString](filemanager.html#readstring){.tsd-kind-icon}
-   [writeJSON](filemanager.html#writejson){.tsd-kind-icon}
-   [writeString](filemanager.html#writestring){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#basepath .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} basePath

::: {.tsd-signature .tsd-kind-icon}
basePath[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [FileManager.d.ts:58](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L58)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The base POSIX-style path to the directory used by this FileManager.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#baseurl .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} baseURL

::: {.tsd-signature .tsd-kind-icon}
baseURL[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [FileManager.d.ts:53](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L53)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The base local URL (`file:///` format) to the directory used by this
FileManager.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lasterror .tsd-anchor}

### lastError

::: {.tsd-signature .tsd-kind-icon}
lastError[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}
:::

-   Defined in
    [FileManager.d.ts:30](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L30)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function fails, this property will contain the last error as a
string message, otherwise it will be `undefined`.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Attribute Methods
-----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getcreationdate .tsd-anchor}

### getCreationDate

-   getCreationDate[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:118](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L118)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get creation date of file at path.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    #### Returns [Date]{.tsd-signature-type} {#returns-date .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getmodificationdate .tsd-anchor}

### getModificationDate

-   getModificationDate[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:125](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L125)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get modification date of file at path.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    #### Returns [Date]{.tsd-signature-type} {#returns-date-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettags .tsd-anchor}

### getTags

-   getTags[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:157](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L157)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get tags on file at path.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-string .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setcreationdate .tsd-anchor}

### setCreationDate

-   setCreationDate[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, date[:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:133](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L133)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Set creation date of file at path. Returns true if successful, false
    if not.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    -   ##### date: [Date]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setmodificationdate .tsd-anchor}

### setModificationDate

-   setModificationDate[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, date[:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:141](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L141)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Set modification date of file at path. Returns true if successful,
    false if not.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    -   ##### date: [Date]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#settags .tsd-anchor}

### setTags

-   setTags[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, tags[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:149](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L149)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Set tags on the file at path.
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    -   ##### tags: [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-2 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Constructors Methods
--------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}isLocal[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[FileManager](filemanager.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:164](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L164)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new FileManager object.
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### isLocal: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        If `true`, the `FileManager` will be using the to the local
        Drafts app documents directory as its root directory, as it
        appears in the \"On my ...\" area in the `Files.app`. If
        `false`, it will use the Drafts5 iCloud folder as its root
        directory.
        :::

    #### Returns [FileManager](filemanager.html){.tsd-signature-type} {#returns-filemanager .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#createcloud .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} createCloud

-   createCloud[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[FileManager](filemanager.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:42](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L42)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Convenience method to create iCloud file manager. iCloud file
    managers work with files in the `iCloud Drive/Drafts` folder
    :::
    :::

    #### Returns [FileManager](filemanager.html){.tsd-signature-type} {#returns-filemanager-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#createforbookmark .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} createForBookmark

-   createForBookmark[(]{.tsd-signature-symbol}bookmark[:
    ]{.tsd-signature-symbol}[Bookmark](bookmark.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[FileManager](filemanager.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:48](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L48)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Convenience method to create a file manager linked to a
    [Bookmark](bookmark.html) object.
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### bookmark: [Bookmark](bookmark.html){.tsd-signature-type}

    #### Returns [FileManager](filemanager.html){.tsd-signature-type} {#returns-filemanager-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#createlocal .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} createLocal

-   createLocal[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[FileManager](filemanager.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:36](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L36)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Convenience method to create local file manager. Note that local
    files are not visible on iOS in the Files app and are only available
    through the use of scripting.
    :::
    :::

    #### Returns [FileManager](filemanager.html){.tsd-signature-type} {#returns-filemanager-3 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Other Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#copyitem .tsd-anchor}

### copyItem

-   copyItem[(]{.tsd-signature-symbol}fromPath[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, toPath[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, overwrite[?:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:111](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L111)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Copy file or directory at `fromPath` to the `toPath`. From and to
    path should be complete paths with file names included.
    :::
    :::

    #### Parameters {#parameters-8 .tsd-parameters-title}

    -   ##### fromPath: [string]{.tsd-signature-type}

    -   ##### toPath: [string]{.tsd-signature-type}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} overwrite: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        If true, replace existing files in at the toPath. If false,
        abort operation if file exists at destination.
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createdirectory .tsd-anchor}

### createDirectory

-   createDirectory[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:95](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L95)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a directory with the specified name in the specified path.
    Returns true if directory successfully created.
    :::
    :::

    #### Parameters {#parameters-9 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

    -   ##### path: [string]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-4 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#exists .tsd-anchor}

### exists

-   exists[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:85](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L85)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Check if a file already exists at the given path.
    :::
    :::

    #### Parameters {#parameters-10 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-5 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#listcontents .tsd-anchor}

### listContents

-   listContents[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:90](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L90)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    List files and directories at the specified path. Array of full path
    will be returned.
    :::
    :::

    #### Parameters {#parameters-11 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-string-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#moveitem .tsd-anchor}

### moveItem

-   moveItem[(]{.tsd-signature-symbol}fromPath[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, toPath[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, overwrite[?:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:103](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L103)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Move file or directory at `fromPath` to the `toPath`. From and to
    path should be complete paths with file names included.
    :::
    :::

    #### Parameters {#parameters-12 .tsd-parameters-title}

    -   ##### fromPath: [string]{.tsd-signature-type}

    -   ##### toPath: [string]{.tsd-signature-type}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} overwrite: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        If true, replace existing files in at the toPath. If false,
        abort operation if file exists at destination.
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-6 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#readjson .tsd-anchor}

### readJSON

-   readJSON[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:75](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L75)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Reads the contents of a JSON formatted file at the path. Returns
    `undefined` value if the file does not exist or could not be read
    and parsed as JSON. Contents could be an object, array of objects,
    etc., depending on the content of the JSON file.
    :::
    :::

    #### Parameters {#parameters-13 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        should begin with a `/` and be relative to the root directory of
        the FileManager.
        :::

    #### Returns [object]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#readstring .tsd-anchor}

### readString

-   readString[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L64)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Reads the contents of the file at the path. Returns `undefined`
    value if the file does not exist or could not be read.
    :::
    :::

    #### Parameters {#parameters-14 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        should begin with a `/` and be relative to the root directory of
        the FileManager.
        :::

    #### Returns [string]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-string-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#writejson .tsd-anchor}

### writeJSON

-   writeJSON[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, content[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:80](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L80)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Write the contents to the path in JSON format. Returns true if
    successful, false if the file could not be written successfully.
    This will override existing files!
    :::
    :::

    #### Parameters {#parameters-15 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    -   ##### content: [object]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-7 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#writestring .tsd-anchor}

### writeString

-   writeString[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, content[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [FileManager.d.ts:69](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/FileManager.d.ts#L69)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Write the contents of the file at the path. Returns true if
    successful, false if the file could not be written successfully.
    This will override existing files!
    :::
    :::

    #### Parameters {#parameters-16 .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

    -   ##### content: [string]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-8 .tsd-returns-title}
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
-   [FileManager](filemanager.html){.tsd-kind-icon}
    -   [basePath](filemanager.html#basepath){.tsd-kind-icon}
    -   [baseURL](filemanager.html#baseurl){.tsd-kind-icon}
    -   [lastError](filemanager.html#lasterror){.tsd-kind-icon}
    -   [copyItem](filemanager.html#copyitem){.tsd-kind-icon}
    -   [createDirectory](filemanager.html#createdirectory){.tsd-kind-icon}
    -   [exists](filemanager.html#exists){.tsd-kind-icon}
    -   [getCreationDate](filemanager.html#getcreationdate){.tsd-kind-icon}
    -   [getModificationDate](filemanager.html#getmodificationdate){.tsd-kind-icon}
    -   [getTags](filemanager.html#gettags){.tsd-kind-icon}
    -   [listContents](filemanager.html#listcontents){.tsd-kind-icon}
    -   [moveItem](filemanager.html#moveitem){.tsd-kind-icon}
    -   [readJSON](filemanager.html#readjson){.tsd-kind-icon}
    -   [readString](filemanager.html#readstring){.tsd-kind-icon}
    -   [setCreationDate](filemanager.html#setcreationdate){.tsd-kind-icon}
    -   [setModificationDate](filemanager.html#setmodificationdate){.tsd-kind-icon}
    -   [setTags](filemanager.html#settags){.tsd-kind-icon}
    -   [writeJSON](filemanager.html#writejson){.tsd-kind-icon}
    -   [writeString](filemanager.html#writestring){.tsd-kind-icon}
    -   [create](filemanager.html#create){.tsd-kind-icon}
    -   [createCloud](filemanager.html#createcloud){.tsd-kind-icon}
    -   [createForBookmark](filemanager.html#createforbookmark){.tsd-kind-icon}
    -   [createLocal](filemanager.html#createlocal){.tsd-kind-icon}

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
