---
{"dg-publish":true,"permalink":"/snippets/app/","dgHomeLink":true,"dgPassFrontmatter":false}
---

app

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
-   [App](app.html)

Class App
=========
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#app){#app}

App
===
:::

Drafts defines a single global `app` object which provides access to
application level functions.

[](#examples){#examples}

### Examples

    // toggle dark-light mode
    if (app.currentThemeMode == 'dark') {
      app.themeMode = 'light';
    }
    else {
      app.themeMode = 'dark';
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [App]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Interface Properties

-   [currentWorkspace](app.html#currentworkspace){.tsd-kind-icon}
-   [isActionListVisible](app.html#isactionlistvisible){.tsd-kind-icon}
-   [isDraftListVisible](app.html#isdraftlistvisible){.tsd-kind-icon}

### System Properties

-   [isIdleDisabled](app.html#isidledisabled){.tsd-kind-icon}
-   [isPro](app.html#ispro){.tsd-kind-icon}
-   [version](app.html#version){.tsd-kind-icon}

### Theme Properties

-   [currentThemeMode](app.html#currentthememode){.tsd-kind-icon}
-   [darkTheme](app.html#darktheme){.tsd-kind-icon}
-   [lightTheme](app.html#lighttheme){.tsd-kind-icon}
-   [themeMode](app.html#thememode){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Deprecated Methods

-   [loadKeyboardActionGroup](app.html#loadkeyboardactiongroup){.tsd-kind-icon}

### Interface Methods

-   [applyWorkspace](app.html#applyworkspace){.tsd-kind-icon}
-   [displaySuccessMessage](app.html#displaysuccessmessage){.tsd-kind-icon}
-   [hideActionList](app.html#hideactionlist){.tsd-kind-icon}
-   [hideDraftList](app.html#hidedraftlist){.tsd-kind-icon}
-   [loadActionBarGroup](app.html#loadactionbargroup){.tsd-kind-icon}
-   [loadActionGroup](app.html#loadactiongroup){.tsd-kind-icon}
-   [openInNewWindow](app.html#openinnewwindow){.tsd-kind-icon}
-   [selectDraft](app.html#selectdraft){.tsd-kind-icon}
-   [showActionList](app.html#showactionlist){.tsd-kind-icon}
-   [showDraftInfo](app.html#showdraftinfo){.tsd-kind-icon}
-   [showDraftList](app.html#showdraftlist){.tsd-kind-icon}
-   [showQuickSearch](app.html#showquicksearch){.tsd-kind-icon}

### Messages Methods

-   [displayErrorMessage](app.html#displayerrormessage){.tsd-kind-icon}
-   [displayInfoMessage](app.html#displayinfomessage){.tsd-kind-icon}
-   [displayWarningMessage](app.html#displaywarningmessage){.tsd-kind-icon}

### Utility Methods

-   [getClipboard](app.html#getclipboard){.tsd-kind-icon}
-   [htmlToClipboard](app.html#htmltoclipboard){.tsd-kind-icon}
-   [openURL](app.html#openurl){.tsd-kind-icon}
-   [queueAction](app.html#queueaction){.tsd-kind-icon}
-   [setClipboard](app.html#setclipboard){.tsd-kind-icon}
-   [setIdleDisabled](app.html#setidledisabled){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Interface Properties
--------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#currentworkspace .tsd-anchor}

### currentWorkspace

::: {.tsd-signature .tsd-kind-icon}
currentWorkspace[:]{.tsd-signature-symbol}
[Workspace](workspace.html){.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:156](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L156)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Returns a workspace object configured like the workspace currently
loaded in the draft list of the active window. Useful when creating
logic which reacts contextually to the workspace loaded.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isactionlistvisible .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} isActionListVisible

::: {.tsd-signature .tsd-kind-icon}
isActionListVisible[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L64)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Is the action list side panel is visible.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isdraftlistvisible .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} isDraftListVisible

::: {.tsd-signature .tsd-kind-icon}
isDraftListVisible[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:58](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L58)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Is the draft list side panel is visible.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
System Properties
-----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isidledisabled .tsd-anchor}

### isIdleDisabled

::: {.tsd-signature .tsd-kind-icon}
isIdleDisabled[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:70](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L70)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Is system sleep timer disabled preventing screen dimming/sleep.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#ispro .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} isPro

::: {.tsd-signature .tsd-kind-icon}
isPro[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:22](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L22)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Returns true if app has an active Drafts Pro subscription.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#version .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} version

::: {.tsd-signature .tsd-kind-icon}
version[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:28](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L28)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Version number of current installation of Drafts.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Theme Properties
----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#currentthememode .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} currentThemeMode

::: {.tsd-signature .tsd-kind-icon}
currentThemeMode[:]{.tsd-signature-symbol}
[\"light\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"dark\"]{.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:52](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L52)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Returns the active theme mode, light or dark, taking into account
automatic switching of themes if active. If writing scripts to branch
logic based on the current mode, this is the best property to use.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#darktheme .tsd-anchor}

### darkTheme

::: {.tsd-signature .tsd-kind-icon}
darkTheme[:]{.tsd-signature-symbol}
[Theme](theme.html){.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:46](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L46)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The current dark mode theme.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lighttheme .tsd-anchor}

### lightTheme

::: {.tsd-signature .tsd-kind-icon}
lightTheme[:]{.tsd-signature-symbol}
[Theme](theme.html){.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:40](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L40)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The current light mode theme.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#thememode .tsd-anchor}

### themeMode

::: {.tsd-signature .tsd-kind-icon}
themeMode[:]{.tsd-signature-symbol} [\"light\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"dark\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"automatic\"]{.tsd-signature-type}
:::

-   Defined in
    [App.d.ts:34](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L34)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Get or set themeMode.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Deprecated Methods
------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#loadkeyboardactiongroup .tsd-anchor}

### loadKeyboardActionGroup

-   loadKeyboardActionGroup[(]{.tsd-signature-symbol}actionGroup[:
    ]{.tsd-signature-symbol}[ActionGroup](actiongroup.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:174](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L174)

    ::: {.tsd-comment .tsd-typography}

    deprecated

    :   replaced by `loadActionBarGroup`.
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### actionGroup: [ActionGroup](actiongroup.html){.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Interface Methods
-----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#applyworkspace .tsd-anchor}

### applyWorkspace

-   applyWorkspace[(]{.tsd-signature-symbol}workspace[?:
    ]{.tsd-signature-symbol}[Workspace](workspace.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:150](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L150)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Apply the Workspace as if it was selected in draft list. Calling
    this function with no arguments will clear filters and apply the
    default workspace.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} workspace: [Workspace](workspace.html){.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#displaysuccessmessage .tsd-anchor}

### displaySuccessMessage

-   displaySuccessMessage[(]{.tsd-signature-symbol}message[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:209](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L209)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Show success banner notification with the message passed.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### message: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#hideactionlist .tsd-anchor}

### hideActionList

-   hideActionList[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:144](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L144)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Close action list side bar.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#hidedraftlist .tsd-anchor}

### hideDraftList

-   hideDraftList[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:113](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L113)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Close draft list side bar.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#loadactionbargroup .tsd-anchor}

### loadActionBarGroup

-   loadActionBarGroup[(]{.tsd-signature-symbol}actionGroup[:
    ]{.tsd-signature-symbol}[ActionGroup](actiongroup.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:168](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L168)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Load the ActionGroup in the action bar below editor.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### actionGroup: [ActionGroup](actiongroup.html){.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#loadactiongroup .tsd-anchor}

### loadActionGroup

-   loadActionGroup[(]{.tsd-signature-symbol}actionGroup[:
    ]{.tsd-signature-symbol}[ActionGroup](actiongroup.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:162](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L162)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Load the ActionGroup in the action list side bar.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### actionGroup: [ActionGroup](actiongroup.html){.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#openinnewwindow .tsd-anchor}

### openInNewWindow

-   openInNewWindow[(]{.tsd-signature-symbol}draft[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:132](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L132)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    If able, open the requested draft in a new window. This method only
    functions on iPad and Mac. The ability to open new windows is not
    available on iPhone.
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### draft: [Draft](draft.html){.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-4 .tsd-returns-title}

    `true` if successful. `false` if unable to open a new window (as on
    iPhone).
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#selectdraft .tsd-anchor}

### selectDraft

-   selectDraft[(]{.tsd-signature-symbol}workspace[?:
    ]{.tsd-signature-symbol}[Workspace](workspace.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:99](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L99)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open draft selection interface and wait for user to select a draft.
    Returns the select draft object, or `undefined` if user cancelled.
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} workspace: [Workspace](workspace.html){.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        If provided, the workspace will define the default filtering,
        display, and sort options for the selection window.
        :::

    #### Returns [Draft](draft.html){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-draft-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#showactionlist .tsd-anchor}

### showActionList

-   showActionList[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:138](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L138)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open action list side bar.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#showdraftinfo .tsd-anchor}

### showDraftInfo

-   showDraftInfo[(]{.tsd-signature-symbol}draft[?:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:125](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L125)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open the \"Get Info\" view for a draft. If no draft is passed, the
    current active draft in the editor will be used.
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} draft: [Draft](draft.html){.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-4 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#showdraftlist .tsd-anchor}

### showDraftList

-   showDraftList[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:107](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L107)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open draft list side bar.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-5 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#showquicksearch .tsd-anchor}

### showQuickSearch

-   showQuickSearch[(]{.tsd-signature-symbol}initialQuery[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:119](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L119)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Open quick search window, optionally providing a initial query
    value.
    :::
    :::

    #### Parameters {#parameters-8 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} initialQuery: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-6 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Messages Methods
----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#displayerrormessage .tsd-anchor}

### displayErrorMessage

-   displayErrorMessage[(]{.tsd-signature-symbol}message[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:224](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L224)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Show error banner notification with the message passed.
    :::
    :::

    #### Parameters {#parameters-9 .tsd-parameters-title}

    -   ##### message: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-7 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#displayinfomessage .tsd-anchor}

### displayInfoMessage

-   displayInfoMessage[(]{.tsd-signature-symbol}message[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:214](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L214)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Show info banner notification with the message passed.
    :::
    :::

    #### Parameters {#parameters-10 .tsd-parameters-title}

    -   ##### message: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-8 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#displaywarningmessage .tsd-anchor}

### displayWarningMessage

-   displayWarningMessage[(]{.tsd-signature-symbol}message[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:219](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L219)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Show warning banner notification with the message passed.
    :::
    :::

    #### Parameters {#parameters-11 .tsd-parameters-title}

    -   ##### message: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-9 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Utility Methods
---------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getclipboard .tsd-anchor}

### getClipboard

-   getClipboard[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:188](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L188)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get current contents of the system clipboard.
    :::
    :::

    #### Returns [string]{.tsd-signature-type} {#returns-string .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#htmltoclipboard .tsd-anchor}

### htmlToClipboard

-   htmlToClipboard[(]{.tsd-signature-symbol}html[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:202](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L202)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Takes HTML string and converts it to rich-text and places it in the
    system clipboard. Returns true if successful, false if an error
    occurred in conversion.
    :::
    :::

    #### Parameters {#parameters-12 .tsd-parameters-title}

    -   ##### html: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        a possibly-valid html string
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-5 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#openurl .tsd-anchor}

### openURL

-   openURL[(]{.tsd-signature-symbol}url[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, useSafari[?:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:78](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L78)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Request system opens the URL passed. Returns true if URL was opened,
    false if the URL was invalid or no available app can open the URL on
    the device.
    :::
    :::

    #### Parameters {#parameters-13 .tsd-parameters-title}

    -   ##### url: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        url to open
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} useSafari: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        whether to use the Safari View Controller (true) or default
        browser (false).
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-6 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#queueaction .tsd-anchor}

### queueAction

-   queueAction[(]{.tsd-signature-symbol}action[:
    ]{.tsd-signature-symbol}[Action](action.html){.tsd-signature-type},
    draft[:
    ]{.tsd-signature-symbol}[Draft](draft.html){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:92](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L92)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Queues an action to run on a draft after the current action is
    complete.

        // lookup action and draft, and queue the action to run
        let a = Action.find("Copy");
        let d = Draft.find("UUID");
        app.queueAction(a, d);
    :::
    :::

    #### Parameters {#parameters-14 .tsd-parameters-title}

    -   ##### action: [Action](action.html){.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Actions can be obtained using the `Action.find(name)` method.
        :::

    -   ##### draft: [Draft](draft.html){.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        A draft object.
        :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-7 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setclipboard .tsd-anchor}

### setClipboard

-   setClipboard[(]{.tsd-signature-symbol}contents[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:195](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L195)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Set the contents of the system clipboard.
    :::
    :::

    #### Parameters {#parameters-15 .tsd-parameters-title}

    -   ##### contents: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-10 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#setidledisabled .tsd-anchor}

### setIdleDisabled

-   setIdleDisabled[(]{.tsd-signature-symbol}isDisabled[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [App.d.ts:180](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/App.d.ts#L180)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Enable and disable the iOS system sleep timer to prevent screen
    dimming/sleep.
    :::
    :::

    #### Parameters {#parameters-16 .tsd-parameters-title}

    -   ##### isDisabled: [boolean]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-11 .tsd-returns-title}
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
-   [App](app.html){.tsd-kind-icon}
    -   [currentThemeMode](app.html#currentthememode){.tsd-kind-icon}
    -   [currentWorkspace](app.html#currentworkspace){.tsd-kind-icon}
    -   [darkTheme](app.html#darktheme){.tsd-kind-icon}
    -   [isActionListVisible](app.html#isactionlistvisible){.tsd-kind-icon}
    -   [isDraftListVisible](app.html#isdraftlistvisible){.tsd-kind-icon}
    -   [isIdleDisabled](app.html#isidledisabled){.tsd-kind-icon}
    -   [isPro](app.html#ispro){.tsd-kind-icon}
    -   [lightTheme](app.html#lighttheme){.tsd-kind-icon}
    -   [themeMode](app.html#thememode){.tsd-kind-icon}
    -   [version](app.html#version){.tsd-kind-icon}
    -   [applyWorkspace](app.html#applyworkspace){.tsd-kind-icon}
    -   [displayErrorMessage](app.html#displayerrormessage){.tsd-kind-icon}
    -   [displayInfoMessage](app.html#displayinfomessage){.tsd-kind-icon}
    -   [displaySuccessMessage](app.html#displaysuccessmessage){.tsd-kind-icon}
    -   [displayWarningMessage](app.html#displaywarningmessage){.tsd-kind-icon}
    -   [getClipboard](app.html#getclipboard){.tsd-kind-icon}
    -   [hideActionList](app.html#hideactionlist){.tsd-kind-icon}
    -   [hideDraftList](app.html#hidedraftlist){.tsd-kind-icon}
    -   [htmlToClipboard](app.html#htmltoclipboard){.tsd-kind-icon}
    -   [loadActionBarGroup](app.html#loadactionbargroup){.tsd-kind-icon}
    -   [loadActionGroup](app.html#loadactiongroup){.tsd-kind-icon}
    -   [loadKeyboardActionGroup](app.html#loadkeyboardactiongroup){.tsd-kind-icon}
    -   [openInNewWindow](app.html#openinnewwindow){.tsd-kind-icon}
    -   [openURL](app.html#openurl){.tsd-kind-icon}
    -   [queueAction](app.html#queueaction){.tsd-kind-icon}
    -   [selectDraft](app.html#selectdraft){.tsd-kind-icon}
    -   [setClipboard](app.html#setclipboard){.tsd-kind-icon}
    -   [setIdleDisabled](app.html#setidledisabled){.tsd-kind-icon}
    -   [showActionList](app.html#showactionlist){.tsd-kind-icon}
    -   [showDraftInfo](app.html#showdraftinfo){.tsd-kind-icon}
    -   [showDraftList](app.html#showdraftlist){.tsd-kind-icon}
    -   [showQuickSearch](app.html#showquicksearch){.tsd-kind-icon}

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
