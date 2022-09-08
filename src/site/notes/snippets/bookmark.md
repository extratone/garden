---
{"dg-publish":true,"permalink":"/snippets/bookmark/","dgHomeLink":true,"dgPassFrontmatter":false}
---

bookmark

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
-   [Bookmark](bookmark.html)

Class Bookmark
==============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#bookmark){#bookmark}

Bookmark
========
:::

Bookmark objects are used to work with folder bookmarks and the
[FileManager](filemanager.html) object to provide access to folders
outside the Drafts App Sandbox. Bookmarks are unique by name. A
user-friendly name should be used, as the first time a bookmark is
required, the user is prompted to select the folder in their file system
to associate with the bookmark, and a useful name can help guide them to
selecting the correct folder.

*Learn more about [Bookmarks in the User
Guide](https://docs.getdrafts.com/docs/settings/bookmarks)*

[](#example){#example}

### Example

    // find or create a named Bookmark
    let bookmark = Bookmark.findOrCreate("My-Folder");
    let fm = FileManager.createForBookmark(bookmark);

    // write to a file at the root of the bookmark folder
    let success = fm.writeString("/ScriptedFile.txt", "This is the file  * content");

    // read from file in bookmarked folder
    let content = fm.readString("/Test Folder/Test.txt")
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Bookmark]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [name](bookmark.html#name){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [forget](bookmark.html#forget){.tsd-kind-icon}
-   [findOrCreate](bookmark.html#findorcreate){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#name .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} name

::: {.tsd-signature .tsd-kind-icon}
name[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Bookmark.d.ts:31](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Bookmark.d.ts#L31)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The name of the bookmark.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#forget .tsd-anchor}

### forget

-   forget[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Bookmark.d.ts:36](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Bookmark.d.ts#L36)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Forget the bookmark, resetting any associated permissions.
    Generally, this would be a function the user performs in the user
    interface, but could be useful in the case of an action which wishes
    to request and use a one-time bookmark and revoke permissions on
    completion of an action.
    :::
    :::

    #### Returns [any]{.tsd-signature-type} {#returns-any .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#findorcreate .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} findOrCreate

-   findOrCreate[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Bookmark](bookmark.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Bookmark.d.ts:26](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Bookmark.d.ts#L26)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get a bookmark object with the specified name. If no bookmark with
    the specified name exists, a new one will be created.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

    #### Returns [Bookmark](bookmark.html){.tsd-signature-type} {#returns-bookmark .tsd-returns-title}
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
-   [Bookmark](bookmark.html){.tsd-kind-icon}
    -   [name](bookmark.html#name){.tsd-kind-icon}
    -   [forget](bookmark.html#forget){.tsd-kind-icon}
    -   [findOrCreate](bookmark.html#findorcreate){.tsd-kind-icon}

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
