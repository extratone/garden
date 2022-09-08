---
{"dg-publish":true,"permalink":"/snippets/workspace/","dgHomeLink":true,"dgPassFrontmatter":false}
---

workspace

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
-   [Workspace](workspace.html)

Class Workspace
===============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#workspace){#workspace}

Workspace
=========
:::

Represents a Workspace. Can be used to inquire and load workspaces and
apply them using methods on the App object.

[](#example-find-and-load-workspace){#example-find-and-load-workspace}

### Example: Find and Load Workspace

    // find workspace and load it in drafts list
    let workspace = Workspace.find("Projects");
    app.applyWorkspace(workspace);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Workspace]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](workspace.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Display Properties

-   [archiveIncludesFlagged](workspace.html#archiveincludesflagged){.tsd-kind-icon}
-   [inboxIncludesFlagged](workspace.html#inboxincludesflagged){.tsd-kind-icon}
-   [loadActionBarGroup](workspace.html#loadactionbargroup){.tsd-kind-icon}
-   [loadActionListGroup](workspace.html#loadactionlistgroup){.tsd-kind-icon}
-   [loadFolder](workspace.html#loadfolder){.tsd-kind-icon}
-   [preferredDarkTheme](workspace.html#preferreddarktheme){.tsd-kind-icon}
-   [preferredLightTheme](workspace.html#preferredlighttheme){.tsd-kind-icon}
-   [showDate](workspace.html#showdate){.tsd-kind-icon}
-   [showLastAction](workspace.html#showlastaction){.tsd-kind-icon}
-   [showPreview](workspace.html#showpreview){.tsd-kind-icon}
-   [showTags](workspace.html#showtags){.tsd-kind-icon}

### Filter Properties

-   [endDate](workspace.html#enddate){.tsd-kind-icon}
-   [queryString](workspace.html#querystring){.tsd-kind-icon}
-   [startDate](workspace.html#startdate){.tsd-kind-icon}
-   [tagFilter](workspace.html#tagfilter){.tsd-kind-icon}
-   [tagFilterRequireAll](workspace.html#tagfilterrequireall){.tsd-kind-icon}

### Identification Properties

-   [installURL](workspace.html#installurl){.tsd-kind-icon}
-   [name](workspace.html#name){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Other Methods

-   [query](workspace.html#query){.tsd-kind-icon}
-   [update](workspace.html#update){.tsd-kind-icon}
-   [create](workspace.html#create){.tsd-kind-icon}
-   [find](workspace.html#find){.tsd-kind-icon}
-   [getAll](workspace.html#getall){.tsd-kind-icon}

### Sort Methods

-   [setAllSort](workspace.html#setallsort){.tsd-kind-icon}
-   [setArchiveSort](workspace.html#setarchivesort){.tsd-kind-icon}
-   [setFlaggedSort](workspace.html#setflaggedsort){.tsd-kind-icon}
-   [setInboxSort](workspace.html#setinboxsort){.tsd-kind-icon}
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

-   new Workspace[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Workspace](workspace.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:177](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L177)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [Workspace](workspace.html){.tsd-signature-type} {#returns-workspace .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Display Properties
------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#archiveincludesflagged .tsd-anchor}

### archiveIncludesFlagged

::: {.tsd-signature .tsd-kind-icon}
archiveIncludesFlagged[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:92](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L92)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Should flagged drafts be included in archive.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#inboxincludesflagged .tsd-anchor}

### inboxIncludesFlagged

::: {.tsd-signature .tsd-kind-icon}
inboxIncludesFlagged[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:86](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L86)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Should flagged drafts be included in inbox.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#loadactionbargroup .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} loadActionBarGroup

::: {.tsd-signature .tsd-kind-icon}
loadActionBarGroup[:]{.tsd-signature-symbol}
[ActionGroup](actiongroup.html){.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:110](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L110)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Action group to load in Action Bar when applying the workspace.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#loadactionlistgroup .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} loadActionListGroup

::: {.tsd-signature .tsd-kind-icon}
loadActionListGroup[:]{.tsd-signature-symbol}
[ActionGroup](actiongroup.html){.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:104](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L104)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Action group to load in action list when applying the workspace.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#loadfolder .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} loadFolder

::: {.tsd-signature .tsd-kind-icon}
loadFolder[:]{.tsd-signature-symbol}
[draftFolderTab](../globals.html#draftfoldertab){.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:98](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L98)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Folder tab to select when applying the workspace.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#preferreddarktheme .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} preferredDarkTheme

::: {.tsd-signature .tsd-kind-icon}
preferredDarkTheme[:]{.tsd-signature-symbol}
[Theme](theme.html){.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:122](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L122)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Preferred dark theme to load when applying the workspace.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#preferredlighttheme .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} preferredLightTheme

::: {.tsd-signature .tsd-kind-icon}
preferredLightTheme[:]{.tsd-signature-symbol}
[Theme](theme.html){.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:116](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L116)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Preferred light theme to load when applying the workspace.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#showdate .tsd-anchor}

### showDate

::: {.tsd-signature .tsd-kind-icon}
showDate[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:68](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L68)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Show date information in list.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#showlastaction .tsd-anchor}

### showLastAction

::: {.tsd-signature .tsd-kind-icon}
showLastAction[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:80](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L80)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Show last logged action for draft in list.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#showpreview .tsd-anchor}

### showPreview

::: {.tsd-signature .tsd-kind-icon}
showPreview[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:62](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L62)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Show preview of draft body in list.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#showtags .tsd-anchor}

### showTags

::: {.tsd-signature .tsd-kind-icon}
showTags[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:74](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L74)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Show draft tags in list.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Filter Properties
-----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#enddate .tsd-anchor}

### endDate

::: {.tsd-signature .tsd-kind-icon}
endDate[:]{.tsd-signature-symbol}
[QueryDate](querydate.html){.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L50)

::: {.tsd-comment .tsd-typography}
::: {.lead}
A [QueryDate](querydate.html) specifying a date which all drafts in the
workspace must be less than or equal to.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#querystring .tsd-anchor}

### queryString

::: {.tsd-signature .tsd-kind-icon}
queryString[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:32](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L32)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Search string to filter results.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#startdate .tsd-anchor}

### startDate

::: {.tsd-signature .tsd-kind-icon}
startDate[:]{.tsd-signature-symbol}
[QueryDate](querydate.html){.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:44](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L44)

::: {.tsd-comment .tsd-typography}
::: {.lead}
A [QueryDate](querydate.html) specifying a date which all drafts in the
workspace must be greater than or equal to.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#tagfilter .tsd-anchor}

### tagFilter

::: {.tsd-signature .tsd-kind-icon}
tagFilter[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:38](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L38)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Comma-delimited list tag string like \"blue, !green\" using \"!\" to
omit a tag.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#tagfilterrequireall .tsd-anchor}

### tagFilterRequireAll

::: {.tsd-signature .tsd-kind-icon}
tagFilterRequireAll[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L56)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If `true`, all (AND) tags in the tag filter must match, if `false` match
any of the tags (OR)
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Identification Properties
-------------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#installurl .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} installURL

::: {.tsd-signature .tsd-kind-icon}
installURL[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:26](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L26)

::: {.tsd-comment .tsd-typography}
::: {.lead}
URL which can be used to install this Workspace in another installation
of Drafts. Useful for sharing and backups.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#name .tsd-anchor}

### name

::: {.tsd-signature .tsd-kind-icon}
name[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Workspace.d.ts:20](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L20)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The name of the workspace.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Other Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#query .tsd-anchor}

### query

-   query[(]{.tsd-signature-symbol}filter[:
    ]{.tsd-signature-symbol}[\"inbox\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"archive\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"flagged\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"trash\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"all\"]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:143](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L143)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Query for a list of drafts contained in the workspace.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### filter: [\"inbox\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"archive\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"flagged\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"trash\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"all\"]{.tsd-signature-type}

    #### Returns [Draft](draft.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-draft .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#update .tsd-anchor}

### update

-   update[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:128](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L128)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Save changes made to the workspace to the database. This must be
    called to save changes.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Workspace](workspace.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:177](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L177)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    create a new workspace object. This is an in-memory object only,
    unless `update()` is called to save the it. The initial state of the
    workspace properties is based on the configuration of the user\'s
    default workspace.
    :::
    :::

    #### Returns [Workspace](workspace.html){.tsd-signature-type} {#returns-workspace-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#find .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} find

-   find[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Workspace](workspace.html){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:192](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L192)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Search for workspace matching the name passed and return it if
    found. Returns undefined if not found.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

    #### Returns [Workspace](workspace.html){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-workspace-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#getall .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} getAll

-   getAll[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Workspace](workspace.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:187](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L187)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get list of all available workspaces.
    :::
    :::

    #### Returns [Workspace](workspace.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-workspace-2 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Sort Methods
------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setallsort .tsd-anchor}

### setAllSort

-   setAllSort[(]{.tsd-signature-symbol}sortBy[:
    ]{.tsd-signature-symbol}[sortBy](){.tsd-signature-type},
    sortDescending[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type},
    sortFlaggedToTop[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:168](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L168)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Set sort order for \"all\" drafts folder.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### sortBy: [sortBy](){.tsd-signature-type}

    -   ##### sortDescending: [boolean]{.tsd-signature-type}

    -   ##### sortFlaggedToTop: [boolean]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setarchivesort .tsd-anchor}

### setArchiveSort

-   setArchiveSort[(]{.tsd-signature-symbol}sortBy[:
    ]{.tsd-signature-symbol}[sortBy](){.tsd-signature-type},
    sortDescending[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type},
    sortFlaggedToTop[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:158](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L158)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Set sort order for archive.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### sortBy: [sortBy](){.tsd-signature-type}

    -   ##### sortDescending: [boolean]{.tsd-signature-type}

    -   ##### sortFlaggedToTop: [boolean]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setflaggedsort .tsd-anchor}

### setFlaggedSort

-   setFlaggedSort[(]{.tsd-signature-symbol}sortBy[:
    ]{.tsd-signature-symbol}[sortBy](){.tsd-signature-type},
    sortDescending[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:149](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L149)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Set sort order for flagged.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### sortBy: [sortBy](){.tsd-signature-type}

    -   ##### sortDescending: [boolean]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setinboxsort .tsd-anchor}

### setInboxSort

-   setInboxSort[(]{.tsd-signature-symbol}sortBy[:
    ]{.tsd-signature-symbol}[sortBy](){.tsd-signature-type},
    sortDescending[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type},
    sortFlaggedToTop[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Workspace.d.ts:134](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Workspace.d.ts#L134)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Set sort order for inbox.
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### sortBy: [sortBy](){.tsd-signature-type}

    -   ##### sortDescending: [boolean]{.tsd-signature-type}

    -   ##### sortFlaggedToTop: [boolean]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-4 .tsd-returns-title}
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
-   [Workspace](workspace.html){.tsd-kind-icon}
    -   [constructor](workspace.html#constructor){.tsd-kind-icon}
    -   [archiveIncludesFlagged](workspace.html#archiveincludesflagged){.tsd-kind-icon}
    -   [endDate](workspace.html#enddate){.tsd-kind-icon}
    -   [inboxIncludesFlagged](workspace.html#inboxincludesflagged){.tsd-kind-icon}
    -   [installURL](workspace.html#installurl){.tsd-kind-icon}
    -   [loadActionBarGroup](workspace.html#loadactionbargroup){.tsd-kind-icon}
    -   [loadActionListGroup](workspace.html#loadactionlistgroup){.tsd-kind-icon}
    -   [loadFolder](workspace.html#loadfolder){.tsd-kind-icon}
    -   [name](workspace.html#name){.tsd-kind-icon}
    -   [preferredDarkTheme](workspace.html#preferreddarktheme){.tsd-kind-icon}
    -   [preferredLightTheme](workspace.html#preferredlighttheme){.tsd-kind-icon}
    -   [queryString](workspace.html#querystring){.tsd-kind-icon}
    -   [showDate](workspace.html#showdate){.tsd-kind-icon}
    -   [showLastAction](workspace.html#showlastaction){.tsd-kind-icon}
    -   [showPreview](workspace.html#showpreview){.tsd-kind-icon}
    -   [showTags](workspace.html#showtags){.tsd-kind-icon}
    -   [startDate](workspace.html#startdate){.tsd-kind-icon}
    -   [tagFilter](workspace.html#tagfilter){.tsd-kind-icon}
    -   [tagFilterRequireAll](workspace.html#tagfilterrequireall){.tsd-kind-icon}
    -   [query](workspace.html#query){.tsd-kind-icon}
    -   [setAllSort](workspace.html#setallsort){.tsd-kind-icon}
    -   [setArchiveSort](workspace.html#setarchivesort){.tsd-kind-icon}
    -   [setFlaggedSort](workspace.html#setflaggedsort){.tsd-kind-icon}
    -   [setInboxSort](workspace.html#setinboxsort){.tsd-kind-icon}
    -   [update](workspace.html#update){.tsd-kind-icon}
    -   [create](workspace.html#create){.tsd-kind-icon}
    -   [find](workspace.html#find){.tsd-kind-icon}
    -   [getAll](workspace.html#getall){.tsd-kind-icon}

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
