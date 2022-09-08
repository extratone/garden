---
{"dg-publish":true,"permalink":"/snippets/editor/","dgHomeLink":true,"dgPassFrontmatter":false}
---

editor

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
-   [Editor](editor.html)

Class Editor
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#editor){#editor}

Editor
======
:::

A global `editor` object is available in all action scripts. This object
allows manipulation of the main editing window in Drafts, altering the
text, text selections, or loading a different draft into the editor,
etc.

Typically scripting actions that work like custom keyboard commands and
similar will utilize the editor functions to manipulate text.

**NOTE:** *Generally speaking, editor methods are best used for quick
text manipulations of the type used in the extended keyboard. Most
substantial updates to draft content are better applied using the
`draft` object.*
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Editor]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Deprecated Properties

-   [focusModeEnabled](editor.html#focusmodeenabled){.tsd-kind-icon}

### Other Properties

-   [isActive](editor.html#isactive){.tsd-kind-icon}
-   [linkModeEnabled](editor.html#linkmodeenabled){.tsd-kind-icon}
-   [navigationMarkers](editor.html#navigationmarkers){.tsd-kind-icon}
-   [pinningEnabled](editor.html#pinningenabled){.tsd-kind-icon}
-   [preferredTabString](editor.html#preferredtabstring){.tsd-kind-icon}
-   [recentDrafts](editor.html#recentdrafts){.tsd-kind-icon}
-   [typewriterScrollingEnabled](editor.html#typewriterscrollingenabled){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [activate](editor.html#activate){.tsd-kind-icon}
-   [arrange](editor.html#arrange){.tsd-kind-icon}
-   [deactivate](editor.html#deactivate){.tsd-kind-icon}
-   [dictate](editor.html#dictate){.tsd-kind-icon}
-   [getLineRange](editor.html#getlinerange){.tsd-kind-icon}
-   [getSelectedLineRange](editor.html#getselectedlinerange){.tsd-kind-icon}
-   [getSelectedRange](editor.html#getselectedrange){.tsd-kind-icon}
-   [getSelectedText](editor.html#getselectedtext){.tsd-kind-icon}
-   [getText](editor.html#gettext){.tsd-kind-icon}
-   [getTextInRange](editor.html#gettextinrange){.tsd-kind-icon}
-   [load](editor.html#load){.tsd-kind-icon}
-   [navigationMarkerAfter](editor.html#navigationmarkerafter){.tsd-kind-icon}
-   [navigationMarkerBefore](editor.html#navigationmarkerbefore){.tsd-kind-icon}
-   [new](editor.html#new){.tsd-kind-icon}
-   [redo](editor.html#redo){.tsd-kind-icon}
-   [save](editor.html#save){.tsd-kind-icon}
-   [scanDocument](editor.html#scandocument){.tsd-kind-icon}
-   [setSelectedRange](editor.html#setselectedrange){.tsd-kind-icon}
-   [setSelectedText](editor.html#setselectedtext){.tsd-kind-icon}
-   [setText](editor.html#settext){.tsd-kind-icon}
-   [setTextInRange](editor.html#settextinrange){.tsd-kind-icon}
-   [showArrange](editor.html#showarrange){.tsd-kind-icon}
-   [showDictate](editor.html#showdictate){.tsd-kind-icon}
-   [showFind](editor.html#showfind){.tsd-kind-icon}
-   [transcribe](editor.html#transcribe){.tsd-kind-icon}
-   [undo](editor.html#undo){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Deprecated Properties
---------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#focusmodeenabled .tsd-anchor}

### focusModeEnabled

::: {.tsd-signature .tsd-kind-icon}
focusModeEnabled[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [Editor.d.ts:46](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L46)

::: {.tsd-comment .tsd-typography}

deprecated

:   replaced by `pinningEnabled`.
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Other Properties
----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isactive .tsd-anchor}

### isActive

::: {.tsd-signature .tsd-kind-icon}
isActive[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Editor.d.ts:71](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L71)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Is editor current focused for editing.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#linkmodeenabled .tsd-anchor}

### linkModeEnabled

::: {.tsd-signature .tsd-kind-icon}
linkModeEnabled[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Editor.d.ts:61](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L61)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Access or set current link mode status.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#navigationmarkers .tsd-anchor}

### navigationMarkers

::: {.tsd-signature .tsd-kind-icon}
navigationMarkers[:]{.tsd-signature-symbol}
[\[]{.tsd-signature-symbol}[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [Editor.d.ts:208](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L208)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of navigation markers in the text. Navigation markers are defined
by the syntax definition in use in the editor, and are used in the
[Navigation](https://docs.getdrafts.com/docs/editor/navigation) feature.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#pinningenabled .tsd-anchor}

### pinningEnabled

::: {.tsd-signature .tsd-kind-icon}
pinningEnabled[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Editor.d.ts:51](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L51)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Access or set current pinning status for editor.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#preferredtabstring .tsd-anchor}

### preferredTabString

::: {.tsd-signature .tsd-kind-icon}
preferredTabString[:]{.tsd-signature-symbol}
[string]{.tsd-signature-type}
:::

-   Defined in
    [Editor.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L56)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Returns the current tab string is use. This could be 2 spaces, 4 spaces,
or `\t` depending on the editor preferences for the current syntax.
Useful in actions, such as indent/outdent actions, which need to insert
or remove indentation and want to match the options of the current
syntax.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#recentdrafts .tsd-anchor}

### recentDrafts

::: {.tsd-signature .tsd-kind-icon}
recentDrafts[:]{.tsd-signature-symbol}
[\[]{.tsd-signature-symbol}[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [Editor.d.ts:76](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L76)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of recent drafts. This is the same list as used in the navigation
features of the editor, and is in reverse order, so that the first index
in the array is the previous draft loaded in the editor.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#typewriterscrollingenabled .tsd-anchor}

### typewriterScrollingEnabled

::: {.tsd-signature .tsd-kind-icon}
typewriterScrollingEnabled[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [Editor.d.ts:66](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L66)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Access or set current typewriter scrolling status.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#activate .tsd-anchor}

### activate

-   activate[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:107](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L107)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Request focus for the editor. This will dismiss other views and show
    the keyboard on the currently loaded draft. Useful if an action
    opens user interface elements or otherwise causes the editor to
    resign focus and you would like to return to editing at the end of
    the action\'s execution.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#arrange .tsd-anchor}

### arrange

-   arrange[(]{.tsd-signature-symbol}text[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:124](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L124)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Opens the arrange mode view with the passed text for arranging.
    Returns the arranged text if the user makes changes and taps
    \"Done\", the original text if the user cancels.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### text: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The text to arrange
        :::

    #### Returns [string]{.tsd-signature-type} {#returns-string .tsd-returns-title}

    String containing result of arrange. If user cancels, it will be the
    same as the original text passed.
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#deactivate .tsd-anchor}

### deactivate

-   deactivate[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:112](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L112)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Resign focus for the editor. If the editor text view is currently
    focused for editing (e.g. showing keyboard), resign focus.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#dictate .tsd-anchor}

### dictate

-   dictate[(]{.tsd-signature-symbol}locale[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:141](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L141)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open dictation interface, and return the result as a string. The
    string will be empty if user cancels.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} locale: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        the preferred locale can be passed in the format \"en-US\" (U.S.
        English), \"it-IT\" (Italian-Italian), \"es-MX\" (Mexican
        Spanish), etc.
        :::

    #### Returns [string]{.tsd-signature-type} {#returns-string-1 .tsd-returns-title}

    The accepted dictation text.
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getlinerange .tsd-anchor}

### getLineRange

-   getLineRange[(]{.tsd-signature-symbol}location[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}, length[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[selectionRange](../globals.html#selectionrange){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:188](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L188)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Expand the range provided to the nearest beginning and end of the
    lines it encompasses.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### location: [number]{.tsd-signature-type}

    -   ##### length: [number]{.tsd-signature-type}

    #### Returns [selectionRange](../globals.html#selectionrange){.tsd-signature-type} {#returns-selectionrange .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getselectedlinerange .tsd-anchor}

### getSelectedLineRange

-   getSelectedLineRange[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[selectionRange](../globals.html#selectionrange){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:178](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L178)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get the current selected text range extended to the beginning and
    end of the lines it encompasses.
    :::
    :::

    #### Returns [selectionRange](../globals.html#selectionrange){.tsd-signature-type} {#returns-selectionrange-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getselectedrange .tsd-anchor}

### getSelectedRange

-   getSelectedRange[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[selectionRange](../globals.html#selectionrange){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:183](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L183)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get text range that was last selected.
    :::
    :::

    #### Returns [selectionRange](../globals.html#selectionrange){.tsd-signature-type} {#returns-selectionrange-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getselectedtext .tsd-anchor}

### getSelectedText

-   getSelectedText[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:168](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L168)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get text range that was last selected.
    :::
    :::

    #### Returns [string]{.tsd-signature-type} {#returns-string-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettext .tsd-anchor}

### getText

-   getText[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:158](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L158)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get the full text currently loaded in the editor.
    :::
    :::

    #### Returns [string]{.tsd-signature-type} {#returns-string-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettextinrange .tsd-anchor}

### getTextInRange

-   getTextInRange[(]{.tsd-signature-symbol}location[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}, length[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:198](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L198)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get the substring in a range from the text in the editor.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### location: [number]{.tsd-signature-type}

    -   ##### length: [number]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type} {#returns-string-4 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#load .tsd-anchor}

### load

-   load[(]{.tsd-signature-symbol}draft[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:87](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L87)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Loads an existing draft into the editor.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### draft: [Draft](draft.html){.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#navigationmarkerafter .tsd-anchor}

### navigationMarkerAfter

-   navigationMarkerAfter[(]{.tsd-signature-symbol}location[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[navigationMarker](../globals.html#navigationmarker){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:213](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L213)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    The next navigation marker in the editor, relative to the character
    location. This is a convenience method to assist in navigating by
    marker.
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### location: [number]{.tsd-signature-type}

    #### Returns [navigationMarker](../globals.html#navigationmarker){.tsd-signature-type} {#returns-navigationmarker .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#navigationmarkerbefore .tsd-anchor}

### navigationMarkerBefore

-   navigationMarkerBefore[(]{.tsd-signature-symbol}location[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[navigationMarker](../globals.html#navigationmarker){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:217](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L217)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    The previous navigation marker in the editor, relative to the
    character location. This is a convenience method to assist in
    navigating by marker.
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### location: [number]{.tsd-signature-type}

    #### Returns [navigationMarker](../globals.html#navigationmarker){.tsd-signature-type} {#returns-navigationmarker-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#new .tsd-anchor}

### new

-   new[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:82](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L82)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new blank draft and loads it into the editor.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#redo .tsd-anchor}

### redo

-   redo[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:102](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L102)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Apply redo action to editor, if one is available.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-4 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#save .tsd-anchor}

### save

-   save[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:92](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L92)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Save any current changes to the draft.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-5 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#scandocument .tsd-anchor}

### scanDocument

-   scanDocument[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:147](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L147)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open document scanning camera to scan documents and OCR, returning
    the result as a string. The string will be empty if user cancels, or
    document scanning is not available.
    :::
    :::

    #### Returns [string]{.tsd-signature-type} {#returns-string-5 .tsd-returns-title}

    The text recognized in the OCR of the scanned document.
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setselectedrange .tsd-anchor}

### setSelectedRange

-   setSelectedRange[(]{.tsd-signature-symbol}location[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}, length[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:193](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L193)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Update the text selection in the editor by passing the start
    location and the length of the new selection.
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### location: [number]{.tsd-signature-type}

    -   ##### length: [number]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-6 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setselectedtext .tsd-anchor}

### setSelectedText

-   setSelectedText[(]{.tsd-signature-symbol}text[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:173](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L173)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Replace the contents of the last text selection with a string.
    :::
    :::

    #### Parameters {#parameters-8 .tsd-parameters-title}

    -   ##### text: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-7 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#settext .tsd-anchor}

### setText

-   setText[(]{.tsd-signature-symbol}text[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:163](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L163)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Replace the contents of the editor with a string.
    :::
    :::

    #### Parameters {#parameters-9 .tsd-parameters-title}

    -   ##### text: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-8 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#settextinrange .tsd-anchor}

### setTextInRange

-   setTextInRange[(]{.tsd-signature-symbol}location[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}, length[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}, text[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:203](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L203)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Replace the text in the passed range with new text.
    :::
    :::

    #### Parameters {#parameters-10 .tsd-parameters-title}

    -   ##### location: [number]{.tsd-signature-type}

    -   ##### length: [number]{.tsd-signature-type}

    -   ##### text: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-9 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#showarrange .tsd-anchor}

### showArrange

-   showArrange[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:117](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L117)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open arrange mode in editor. This is a non-blocking method and
    returns immediately. It is intended only to mimic the tapping of the
    arrange button. Use `editor.arrange(text)` to wait for a result.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-10 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#showdictate .tsd-anchor}

### showDictate

-   showDictate[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:134](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L134)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open dictation mode in editor. This is a non-blocking method and
    returns immediately. It is intended only to mimic the tapping of the
    dictate button. Use `editor.dictate()` to wait for a result and use
    it in further scripting.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-11 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#showfind .tsd-anchor}

### showFind

-   showFind[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:129](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L129)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open find mode in editor.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-12 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#transcribe .tsd-anchor}

### transcribe

-   transcribe[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:153](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L153)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open Opens audio transcription window. If file is selected and
    transcribed, returns text.
    :::
    :::

    #### Returns [string]{.tsd-signature-type} {#returns-string-6 .tsd-returns-title}

    The text recognized in the audio transcription.
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#undo .tsd-anchor}

### undo

-   undo[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Editor.d.ts:97](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Editor.d.ts#L97)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Apply undo action to editor, if one is available.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-13 .tsd-returns-title}
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
-   [Editor](editor.html){.tsd-kind-icon}
    -   [focusModeEnabled](editor.html#focusmodeenabled){.tsd-kind-icon}
    -   [isActive](editor.html#isactive){.tsd-kind-icon}
    -   [linkModeEnabled](editor.html#linkmodeenabled){.tsd-kind-icon}
    -   [navigationMarkers](editor.html#navigationmarkers){.tsd-kind-icon}
    -   [pinningEnabled](editor.html#pinningenabled){.tsd-kind-icon}
    -   [preferredTabString](editor.html#preferredtabstring){.tsd-kind-icon}
    -   [recentDrafts](editor.html#recentdrafts){.tsd-kind-icon}
    -   [typewriterScrollingEnabled](editor.html#typewriterscrollingenabled){.tsd-kind-icon}
    -   [activate](editor.html#activate){.tsd-kind-icon}
    -   [arrange](editor.html#arrange){.tsd-kind-icon}
    -   [deactivate](editor.html#deactivate){.tsd-kind-icon}
    -   [dictate](editor.html#dictate){.tsd-kind-icon}
    -   [getLineRange](editor.html#getlinerange){.tsd-kind-icon}
    -   [getSelectedLineRange](editor.html#getselectedlinerange){.tsd-kind-icon}
    -   [getSelectedRange](editor.html#getselectedrange){.tsd-kind-icon}
    -   [getSelectedText](editor.html#getselectedtext){.tsd-kind-icon}
    -   [getText](editor.html#gettext){.tsd-kind-icon}
    -   [getTextInRange](editor.html#gettextinrange){.tsd-kind-icon}
    -   [load](editor.html#load){.tsd-kind-icon}
    -   [navigationMarkerAfter](editor.html#navigationmarkerafter){.tsd-kind-icon}
    -   [navigationMarkerBefore](editor.html#navigationmarkerbefore){.tsd-kind-icon}
    -   [new](editor.html#new){.tsd-kind-icon}
    -   [redo](editor.html#redo){.tsd-kind-icon}
    -   [save](editor.html#save){.tsd-kind-icon}
    -   [scanDocument](editor.html#scandocument){.tsd-kind-icon}
    -   [setSelectedRange](editor.html#setselectedrange){.tsd-kind-icon}
    -   [setSelectedText](editor.html#setselectedtext){.tsd-kind-icon}
    -   [setText](editor.html#settext){.tsd-kind-icon}
    -   [setTextInRange](editor.html#settextinrange){.tsd-kind-icon}
    -   [showArrange](editor.html#showarrange){.tsd-kind-icon}
    -   [showDictate](editor.html#showdictate){.tsd-kind-icon}
    -   [showFind](editor.html#showfind){.tsd-kind-icon}
    -   [transcribe](editor.html#transcribe){.tsd-kind-icon}
    -   [undo](editor.html#undo){.tsd-kind-icon}

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
