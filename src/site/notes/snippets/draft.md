---
{"dg-publish":true,"permalink":"/snippets/draft/","dgHomeLink":true,"dgPassFrontmatter":false}
---

draft

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
-   [Draft](draft.html)

Class Draft
===========
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#draft){#draft}

Draft
=====
:::

The Draft object represents a single draft. When an action is run, the
current draft is available as the global variable `draft`. Scripts can
also create new drafts, access and set values, and update the draft to
persist changes.

[](#example-creating-a-draft){#example-creating-a-draft}

### Example: Creating a draft

    // create a new draft, assign content and save it
    let d = new Draft();
    d.content = "My new draft";
    d.addTag("personal");
    d.update();

[](#example-querying-drafts){#example-querying-drafts}

### Example: Querying drafts

    // query a list of drafts in the inbox with the tag "blue"
    let drafts = Draft.query("", "inbox", ["blue"])
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Draft]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](draft.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### ActionLog Properties

-   [actionLogs](draft.html#actionlogs){.tsd-kind-icon}

### Date Properties

-   [createdAt](draft.html#createdat){.tsd-kind-icon}
-   [modifiedAt](draft.html#modifiedat){.tsd-kind-icon}

### Deprecated Properties

-   [languageGrammar](draft.html#languagegrammar){.tsd-kind-icon}

### Location Properties

-   [createdLatitude](draft.html#createdlatitude){.tsd-kind-icon}
-   [createdLongitude](draft.html#createdlongitude){.tsd-kind-icon}
-   [modifiedLatitude](draft.html#modifiedlatitude){.tsd-kind-icon}
-   [modifiedLongitude](draft.html#modifiedlongitude){.tsd-kind-icon}

### Other Properties

-   [content](draft.html#content){.tsd-kind-icon}
-   [displayTitle](draft.html#displaytitle){.tsd-kind-icon}
-   [isArchived](draft.html#isarchived){.tsd-kind-icon}
-   [isFlagged](draft.html#isflagged){.tsd-kind-icon}
-   [isTrashed](draft.html#istrashed){.tsd-kind-icon}
-   [lines](draft.html#lines){.tsd-kind-icon}
-   [permalink](draft.html#permalink){.tsd-kind-icon}
-   [selectionLength](draft.html#selectionlength){.tsd-kind-icon}
-   [selectionStart](draft.html#selectionstart){.tsd-kind-icon}
-   [syntax](draft.html#syntax){.tsd-kind-icon}
-   [title](draft.html#title){.tsd-kind-icon}
-   [uuid](draft.html#uuid){.tsd-kind-icon}

### Tag Properties

-   [tags](draft.html#tags){.tsd-kind-icon}

### Version Properties

-   [versions](draft.html#versions){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Other Methods

-   [append](draft.html#append){.tsd-kind-icon}
-   [bodyPreview](draft.html#bodypreview){.tsd-kind-icon}
-   [prepend](draft.html#prepend){.tsd-kind-icon}
-   [update](draft.html#update){.tsd-kind-icon}
-   [create](draft.html#create){.tsd-kind-icon}

### Querying Methods

-   [find](draft.html#find){.tsd-kind-icon}
-   [query](draft.html#query){.tsd-kind-icon}
-   [queryByTitle](draft.html#querybytitle){.tsd-kind-icon}

### Tag Methods

-   [addTag](draft.html#addtag){.tsd-kind-icon}
-   [hasTag](draft.html#hastag){.tsd-kind-icon}
-   [removeTag](draft.html#removetag){.tsd-kind-icon}
-   [recentTags](draft.html#recenttags){.tsd-kind-icon}

### Template Methods

-   [getTemplateTag](draft.html#gettemplatetag){.tsd-kind-icon}
-   [processMustacheTemplate](draft.html#processmustachetemplate){.tsd-kind-icon}
-   [processTemplate](draft.html#processtemplate){.tsd-kind-icon}
-   [setTemplateTag](draft.html#settemplatetag){.tsd-kind-icon}

### Version Methods

-   [saveVersion](draft.html#saveversion){.tsd-kind-icon}
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

-   new Draft[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:24](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L24)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [Draft](draft.html){.tsd-signature-type} {#returns-draft .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
ActionLog Properties
--------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#actionlogs .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} actionLogs

::: {.tsd-signature .tsd-kind-icon}
actionLogs[:]{.tsd-signature-symbol}
[ActionLog](actionlog.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [Draft.d.ts:213](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L213)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of versions representing the entire saved version history for this
draft.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Date Properties
---------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#createdat .tsd-anchor}

### createdAt

::: {.tsd-signature .tsd-kind-icon}
createdAt[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:113](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L113)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Date the draft was created. This property is generally maintained by
Drafts automatically and is it not recommended it be set directly unless
needed to maintain information from an external source when importing.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#modifiedat .tsd-anchor}

### modifiedAt

::: {.tsd-signature .tsd-kind-icon}
modifiedAt[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:128](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L128)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Date the draft was last modified. This property is generally maintained
by Drafts automatically and is it not recommended it be set directly
unless needed to maintain information from an external source when
importing.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Deprecated Properties
---------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#languagegrammar .tsd-anchor}

### languageGrammar

::: {.tsd-signature .tsd-kind-icon}
languageGrammar[:]{.tsd-signature-symbol} [\"Plain
Text\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"Markdown\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"Taskpaper\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"JavaScript\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"Simple List\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"MultiMarkdown\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"GitHub Markdown\"]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L64)

::: {.tsd-comment .tsd-typography}

deprecated

:   use `syntax` property.
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Location Properties
-------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#createdlatitude .tsd-anchor}

### createdLatitude

::: {.tsd-signature .tsd-kind-icon}
createdLatitude[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:123](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L123)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Numeric latitude where the draft was created. This value will be `0` if
no location information was available.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#createdlongitude .tsd-anchor}

### createdLongitude

::: {.tsd-signature .tsd-kind-icon}
createdLongitude[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:118](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L118)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Numeric longitude where the draft was created. This value will be `0` if
no location information was available.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#modifiedlatitude .tsd-anchor}

### modifiedLatitude

::: {.tsd-signature .tsd-kind-icon}
modifiedLatitude[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:138](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L138)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Numeric longitude where the draft was last modified. This value will be
`0` if no location information was available.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#modifiedlongitude .tsd-anchor}

### modifiedLongitude

::: {.tsd-signature .tsd-kind-icon}
modifiedLongitude[:]{.tsd-signature-symbol}
[number]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:133](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L133)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Numeric longitude where the draft was last modified. This value will be
`0` if no location information was available.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Other Properties
----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#content .tsd-anchor}

### content

::: {.tsd-signature .tsd-kind-icon}
content[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:38](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L38)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The full text content.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#displaytitle .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} displayTitle

::: {.tsd-signature .tsd-kind-icon}
displayTitle[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:48](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L48)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Generally, the first line of the draft, but cleaned up as it would be
displayed in the draft list in the user interface, removing Markdown
header characters, etc.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isarchived .tsd-anchor}

### isArchived

::: {.tsd-signature .tsd-kind-icon}
isArchived[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:97](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L97)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Is the draft current in the archive. If `false`, the draft is in the
inbox.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isflagged .tsd-anchor}

### isFlagged

::: {.tsd-signature .tsd-kind-icon}
isFlagged[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:107](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L107)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Current flagged status.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#istrashed .tsd-anchor}

### isTrashed

::: {.tsd-signature .tsd-kind-icon}
isTrashed[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:102](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L102)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Is the draft currently in the trash.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lines .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} lines

::: {.tsd-signature .tsd-kind-icon}
lines[:]{.tsd-signature-symbol}
[\[]{.tsd-signature-symbol}[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [Draft.d.ts:53](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L53)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The lines of content separated into an array on `\n` line feeds. This is
a convenience method an equivalent to `content.split('\n');`
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#permalink .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} permalink

::: {.tsd-signature .tsd-kind-icon}
permalink[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:143](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L143)

::: {.tsd-comment .tsd-typography}
::: {.lead}
URL which can be used to open the draft. URLs are cross-platform, but
specific to an individual user\'s drafts datastore.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#selectionlength .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} selectionLength

::: {.tsd-signature .tsd-kind-icon}
selectionLength[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:86](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L86)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The length of the last text selection.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#selectionstart .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} selectionStart

::: {.tsd-signature .tsd-kind-icon}
selectionStart[:]{.tsd-signature-symbol} [number]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:81](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L81)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The index location in the string of the beginning of the last text
selection.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#syntax .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} syntax

::: {.tsd-signature .tsd-kind-icon}
syntax[:]{.tsd-signature-symbol}
[Syntax](syntax.html){.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:76](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L76)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The syntax definition used when displaying this draft in the editor.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#title .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} title

::: {.tsd-signature .tsd-kind-icon}
title[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:43](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L43)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The first line.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#uuid .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} uuid

::: {.tsd-signature .tsd-kind-icon}
uuid[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Draft.d.ts:33](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L33)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Unique identifier.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Tag Properties
--------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#tags .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} tags

::: {.tsd-signature .tsd-kind-icon}
tags[:]{.tsd-signature-symbol}
[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [Draft.d.ts:92](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L92)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of string tag names assigned.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Version Properties
------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#versions .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} versions

::: {.tsd-signature .tsd-kind-icon}
versions[:]{.tsd-signature-symbol}
[Version](version.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [Draft.d.ts:219](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L219)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of versions representing the entire saved version history for this
draft.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Other Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#append .tsd-anchor}

### append

-   append[(]{.tsd-signature-symbol}text[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, separator[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:200](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L200)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Append text to the end of the draft\'s `content`. This is a
    convenience function.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### text: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The text to append
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} separator: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        An optional separator string to use between content and added
        text. Defaults to a single line feed.
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#bodypreview .tsd-anchor}

### bodyPreview

-   bodyPreview[(]{.tsd-signature-symbol}maxLength[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:58](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L58)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Return the a trimmed display version of the \"body\" of the draft
    (content after first line), similar to what is displayed as a
    preview in the draft list.\_
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### maxLength: [number]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type} {#returns-string .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#prepend .tsd-anchor}

### prepend

-   prepend[(]{.tsd-signature-symbol}text[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, separator[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:207](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L207)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Prepend text to the beginning of the draft\'s `content`. This is a
    convenience function.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### text: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The text to prepend
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} separator: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        An optional separator string to use between content and added
        text. Defaults to a single line feed.
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-1 .tsd-returns-title}
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
        [Draft.d.ts:148](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L148)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Save changes made to the draft to the database. *`update()` must be
    called to save changes made to a draft.*
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:230](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L230)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a new draft object. This is an in-memory object only, unless
    \"update()\" is called to save the draft.
    :::
    :::

    #### Returns [Draft](draft.html){.tsd-signature-type} {#returns-draft-1 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Querying Methods
----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#find .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} find

-   find[(]{.tsd-signature-symbol}uuid[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:236](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L236)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Find an existing draft based on UUID.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### uuid: [string]{.tsd-signature-type}

    #### Returns [Draft](draft.html){.tsd-signature-type} {#returns-draft-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#query .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} query

-   query[(]{.tsd-signature-symbol}queryString[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, filter[:
    ]{.tsd-signature-symbol}[\"inbox\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"archive\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"flagged\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"trash\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"all\"]{.tsd-signature-type}, tags[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol},
    omitTags[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol},
    sort[: ]{.tsd-signature-symbol}[\"created\"]{.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[\"modified\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"accessed\"]{.tsd-signature-type},
    sortDescending[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type},
    sortFlaggedToTop[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:249](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L249)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Perform a search for drafts and return an array of matching draft
    objects.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### queryString: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Search string, as you would type in the search box in the draft
        list. Will find only drafts with a matching string in their
        contents. Use empty string (`""`) not to filter.
        :::

    -   ##### filter: [\"inbox\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"archive\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"flagged\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"trash\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"all\"]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Filter by one of the allowed values
        :::

    -   ##### tags: [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        Results will only include drafts with one or more of these tags
        assigned.
        :::

    -   ##### omitTags: [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        Results will omit drafts with any of these tags assigned.
        :::

    -   ##### sort: [\"created\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"modified\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"accessed\"]{.tsd-signature-type}

    -   ##### sortDescending: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        If `true`, sort descending. Defaults to `false`.
        :::

    -   ##### sortFlaggedToTop: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        If `true`, sort flagged drafts to beginning. Defaults to
        `false`.
        :::

    #### Returns [Draft](draft.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-draft-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#querybytitle .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} queryByTitle

-   queryByTitle[(]{.tsd-signature-symbol}title[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:263](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L263)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Search for drafts containing the title string in the first line of
    their content. This mimics the logic used by the `/open?title=Title`
    URL scheme to locate drafts by title when triggering embedded
    [cross-links](https://docs.getdrafts.com/docs/drafts/cross-linking).
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### title: [string]{.tsd-signature-type}

    #### Returns [Draft](draft.html){.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-draft-4 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Tag Methods
-----------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addtag .tsd-anchor}

### addTag

-   addTag[(]{.tsd-signature-symbol}tag[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:154](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L154)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Assign a tag
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### tag: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#hastag .tsd-anchor}

### hasTag

-   hasTag[(]{.tsd-signature-symbol}tag[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:166](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L166)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Check whether a tag is currently assigned to the draft.
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### tag: [string]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#removetag .tsd-anchor}

### removeTag

-   removeTag[(]{.tsd-signature-symbol}tag[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:160](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L160)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Remove a tag if it is assigned to the draft.
    :::
    :::

    #### Parameters {#parameters-8 .tsd-parameters-title}

    -   ##### tag: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-4 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#recenttags .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} recentTags

-   recentTags[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:269](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L269)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Return array of recently used tags. Helpful for building prompts to
    select tags.
    :::
    :::

    #### Returns [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-string-1 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Template Methods
----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettemplatetag .tsd-anchor}

### getTemplateTag

-   getTemplateTag[(]{.tsd-signature-symbol}tagName[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:193](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L193)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get the current value of a custom template tag.
    :::
    :::

    #### Parameters {#parameters-9 .tsd-parameters-title}

    -   ##### tagName: [string]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type} {#returns-string-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#processmustachetemplate .tsd-anchor}

### processMustacheTemplate

-   processMustacheTemplate[(]{.tsd-signature-symbol}template[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type},
    additionalValues[:
    ]{.tsd-signature-symbol}[Object]{.tsd-signature-type}, partials[:
    ]{.tsd-signature-symbol}[Object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:181](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L181)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Runs the template string through the [Mustache
    template](https://docs.getdrafts.com/docs/actions/templates/mustache-templates)
    engine to evaluate tags. Allows additional values and partials to be
    provided to the context.
    :::
    :::

    #### Parameters {#parameters-10 .tsd-parameters-title}

    -   ##### template: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Template string
        :::

    -   ##### additionalValues: [Object]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        An object containing additional values you wish to make
        available in the Mustache context.
        :::

    -   ##### partials: [Object]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        An object containing string keys and values which will contain
        additional templates you which to make available for use as
        partials and layouts.
        :::

    #### Returns [string]{.tsd-signature-type} {#returns-string-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#processtemplate .tsd-anchor}

### processTemplate

-   processTemplate[(]{.tsd-signature-symbol}template[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:172](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L172)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Runs the template string through the [Drafts
    Template](https://docs.getdrafts.com/docs/actions/templates/drafts-templates)
    engine to evaluate tags.
    :::
    :::

    #### Parameters {#parameters-11 .tsd-parameters-title}

    -   ##### template: [string]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type} {#returns-string-4 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#settemplatetag .tsd-anchor}

### setTemplateTag

-   setTemplateTag[(]{.tsd-signature-symbol}tagName[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, value[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:187](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L187)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Set a custom template tag value for use in templates. For example,
    calling `setTemplateTag("mytag", "mytext")` will create a tag
    `[[mytag]]`, which subsequent action steps in the same action can
    use in their templates. These values are also available in Mustache
    templates, but as `{{mytag}}`.
    :::
    :::

    #### Parameters {#parameters-12 .tsd-parameters-title}

    -   ##### tagName: [string]{.tsd-signature-type}

    -   ##### value: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-5 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Version Methods
---------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#saveversion .tsd-anchor}

### saveVersion

-   saveVersion[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Draft.d.ts:225](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Draft.d.ts#L225)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a version in the version history representing the current
    state of the draft.
    :::
    :::

    #### Returns [any]{.tsd-signature-type} {#returns-any .tsd-returns-title}
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
-   [Draft](draft.html){.tsd-kind-icon}
    -   [constructor](draft.html#constructor){.tsd-kind-icon}
    -   [actionLogs](draft.html#actionlogs){.tsd-kind-icon}
    -   [content](draft.html#content){.tsd-kind-icon}
    -   [createdAt](draft.html#createdat){.tsd-kind-icon}
    -   [createdLatitude](draft.html#createdlatitude){.tsd-kind-icon}
    -   [createdLongitude](draft.html#createdlongitude){.tsd-kind-icon}
    -   [displayTitle](draft.html#displaytitle){.tsd-kind-icon}
    -   [isArchived](draft.html#isarchived){.tsd-kind-icon}
    -   [isFlagged](draft.html#isflagged){.tsd-kind-icon}
    -   [isTrashed](draft.html#istrashed){.tsd-kind-icon}
    -   [languageGrammar](draft.html#languagegrammar){.tsd-kind-icon}
    -   [lines](draft.html#lines){.tsd-kind-icon}
    -   [modifiedAt](draft.html#modifiedat){.tsd-kind-icon}
    -   [modifiedLatitude](draft.html#modifiedlatitude){.tsd-kind-icon}
    -   [modifiedLongitude](draft.html#modifiedlongitude){.tsd-kind-icon}
    -   [permalink](draft.html#permalink){.tsd-kind-icon}
    -   [selectionLength](draft.html#selectionlength){.tsd-kind-icon}
    -   [selectionStart](draft.html#selectionstart){.tsd-kind-icon}
    -   [syntax](draft.html#syntax){.tsd-kind-icon}
    -   [tags](draft.html#tags){.tsd-kind-icon}
    -   [title](draft.html#title){.tsd-kind-icon}
    -   [uuid](draft.html#uuid){.tsd-kind-icon}
    -   [versions](draft.html#versions){.tsd-kind-icon}
    -   [addTag](draft.html#addtag){.tsd-kind-icon}
    -   [append](draft.html#append){.tsd-kind-icon}
    -   [bodyPreview](draft.html#bodypreview){.tsd-kind-icon}
    -   [getTemplateTag](draft.html#gettemplatetag){.tsd-kind-icon}
    -   [hasTag](draft.html#hastag){.tsd-kind-icon}
    -   [prepend](draft.html#prepend){.tsd-kind-icon}
    -   [processMustacheTemplate](draft.html#processmustachetemplate){.tsd-kind-icon}
    -   [processTemplate](draft.html#processtemplate){.tsd-kind-icon}
    -   [removeTag](draft.html#removetag){.tsd-kind-icon}
    -   [saveVersion](draft.html#saveversion){.tsd-kind-icon}
    -   [setTemplateTag](draft.html#settemplatetag){.tsd-kind-icon}
    -   [update](draft.html#update){.tsd-kind-icon}
    -   [create](draft.html#create){.tsd-kind-icon}
    -   [find](draft.html#find){.tsd-kind-icon}
    -   [query](draft.html#query){.tsd-kind-icon}
    -   [queryByTitle](draft.html#querybytitle){.tsd-kind-icon}
    -   [recentTags](draft.html#recenttags){.tsd-kind-icon}

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
