---
{"dg-publish":true,"permalink":"/snippets/prompt/","dgHomeLink":true,"dgPassFrontmatter":false}
---

prompt

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
-   [Prompt](prompt.html)

Class Prompt
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#prompt){#prompt}

Prompt
======
:::

Prompts allow the creation and display of custom dialogs to request
information or confirmation from the user.

[](#example){#example}

### Example

    var p = Prompt.create();

    p.title = "Hello";
    p.message = "World!";

    p.addTextField("textFieldName", "Label", "");

    p.addDatePicker("myDate", "Start date", new Date(), {
      "mode": "date"
    });
    p.addButton("First");
    p.addButton("Second");

    var didSelect = p.show();

    var textFieldContents = p.fieldValues["textFieldName"];
    var startDate = p.fieldValues["myDate"];

    if (p.buttonPressed == "First") {
      // do something
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Prompt]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](prompt.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Display Properties

-   [isCancellable](prompt.html#iscancellable){.tsd-kind-icon}
-   [message](prompt.html#message){.tsd-kind-icon}
-   [title](prompt.html#title){.tsd-kind-icon}

### Result Properties

-   [buttonPressed](prompt.html#buttonpressed){.tsd-kind-icon}
-   [fieldValues](prompt.html#fieldvalues){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Field Methods

-   [addButton](prompt.html#addbutton){.tsd-kind-icon}
-   [addDatePicker](prompt.html#adddatepicker){.tsd-kind-icon}
-   [addLabel](prompt.html#addlabel){.tsd-kind-icon}
-   [addPasswordField](prompt.html#addpasswordfield){.tsd-kind-icon}
-   [addPicker](prompt.html#addpicker){.tsd-kind-icon}
-   [addSelect](prompt.html#addselect){.tsd-kind-icon}
-   [addSwitch](prompt.html#addswitch){.tsd-kind-icon}
-   [addTextField](prompt.html#addtextfield){.tsd-kind-icon}
-   [addTextView](prompt.html#addtextview){.tsd-kind-icon}

### Other Methods

-   [show](prompt.html#show){.tsd-kind-icon}
-   [create](prompt.html#create){.tsd-kind-icon}
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

-   new Prompt[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Prompt](prompt.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:231](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L231)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [Prompt](prompt.html){.tsd-signature-type} {#returns-prompt .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Display Properties
------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#iscancellable .tsd-anchor}

### isCancellable

::: {.tsd-signature .tsd-kind-icon}
isCancellable[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Prompt.d.ts:63](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L63)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If true, a \"Cancel\" button will be included in the dialog. Defaults to
`true`. If the user selects the cancel button, the `show()` method will
return `false`. If `false`, no cancel button will be displayed and the
user must select one of the button name options.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#message .tsd-anchor}

### message

::: {.tsd-signature .tsd-kind-icon}
message[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Prompt.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L57)

::: {.tsd-comment .tsd-typography}
::: {.lead}
A longer message explaining the purpose of the dialog, if needed.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#title .tsd-anchor}

### title

::: {.tsd-signature .tsd-kind-icon}
title[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Prompt.d.ts:51](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L51)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Short title.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Result Properties
-----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#buttonpressed .tsd-anchor}

### buttonPressed

::: {.tsd-signature .tsd-kind-icon}
buttonPressed[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Prompt.d.ts:75](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L75)

::: {.tsd-comment .tsd-typography}
::: {.lead}
After the `show()` method is called, this property will contain the name
of the button selected by the user.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#fieldvalues .tsd-anchor}

### fieldValues

::: {.tsd-signature .tsd-kind-icon}
fieldValues[:]{.tsd-signature-symbol} [{}]{.tsd-signature-symbol}
:::

-   Defined in
    [Prompt.d.ts:69](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L69)

::: {.tsd-comment .tsd-typography}
::: {.lead}
After the `show()` method is called, this property will contain values
from any fields added to the prompt. The dictionary keys will be the
names of the fields as passed in when they were created, and the value
will be the current contents of that field. They type of data depends on
the type of field.
:::
:::

::: {.tsd-type-declaration}
#### Type declaration

-   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[any]{.tsd-signature-type}
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Field Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addbutton .tsd-anchor}

### addButton

-   addButton[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, value[?:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}, isDefault[?:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:221](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L221)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a button to the array of buttons to be displayed. All buttons
    should be created before calling `show()`.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} value: [object]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        only needed to associate a different value than will be
        displayed in the button. For example, if you call
        `prompt.addButton("First Button", 1)`, after calling
        `prompt.show()` if that button is pressed, the
        `prompt.buttonPressed` will contain the number value `1`.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} isDefault: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        used to specify a single button which will be pinned to the
        bottom of the prompt and respond to `cmd + return` as the
        default button. If only one button is added to a prompt, it is
        assumed to be the default.
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#adddatepicker .tsd-anchor}

### addDatePicker

-   addDatePicker[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, initialDate[:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}, options[?:
    ]{.tsd-signature-symbol}[{ ]{.tsd-signature-symbol}maximumDate[?:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}[;
    ]{.tsd-signature-symbol}minimumDate[?:
    ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}[;
    ]{.tsd-signature-symbol}minuteInterval[?:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[;
    ]{.tsd-signature-symbol}mode[?:
    ]{.tsd-signature-symbol}[\"date\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"time\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"dateAndTime\"]{.tsd-signature-type}[
    }]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:170](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L170)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a date and/or time picker to the prompt, with the arguments as
    below. The `fieldValues` entry for this will be a date object.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Identifier for the field. This will be used as the key in the
        `fieldValues` dictionary to access the contents of the field
        after calling `show()`.
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        User-friendly text label to place next to the field.
        :::

    -   ##### initialDate: [Date]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The initial date to selected for the field. Minimum and maximum
        values should be defined in options.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} options: [{ ]{.tsd-signature-symbol}maximumDate[?: ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}[; ]{.tsd-signature-symbol}minimumDate[?: ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}[; ]{.tsd-signature-symbol}minuteInterval[?: ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[; ]{.tsd-signature-symbol}mode[?: ]{.tsd-signature-symbol}[\"date\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"time\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"dateAndTime\"]{.tsd-signature-type}[ }]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        A dictionary of options for configuring the text field.
        :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} maximumDate[?: ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} minimumDate[?: ]{.tsd-signature-symbol}[Date]{.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} minuteInterval[?: ]{.tsd-signature-symbol}[number]{.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} mode[?: ]{.tsd-signature-symbol}[\"date\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"time\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"dateAndTime\"]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addlabel .tsd-anchor}

### addLabel

-   addLabel[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[?:
    ]{.tsd-signature-symbol}[{ ]{.tsd-signature-symbol}textSize[?:
    ]{.tsd-signature-symbol}[\"body\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"caption\"]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[\"headline\"]{.tsd-signature-type}[
    }]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:84](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L84)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add an information text label to the prompt.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Identifier for the field.
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The text of the label.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} options: [{ ]{.tsd-signature-symbol}textSize[?: ]{.tsd-signature-symbol}[\"body\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"caption\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"headline\"]{.tsd-signature-type}[ }]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        A dictionary of options for configuring the text field.
        :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} textSize[?: ]{.tsd-signature-symbol}[\"body\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"caption\"]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[\"headline\"]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addpasswordfield .tsd-anchor}

### addPasswordField

-   addPasswordField[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type},
    initialValue[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:151](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L151)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Same as addTextField, but the input field will be password masked.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

    -   ##### label: [string]{.tsd-signature-type}

    -   ##### initialValue: [string]{.tsd-signature-type}

    #### Returns [void]{.tsd-signature-type} {#returns-void-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addpicker .tsd-anchor}

### addPicker

-   addPicker[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, columns[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[\[\]]{.tsd-signature-symbol},
    selectedRows[:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:190](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L190)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a picker to the prompt, with the arguments as below. Picker can
    contain multiple rows. The `fieldValues` entry for this will be a
    array of selected index values object.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Identifier for the field. This will be used as the key in the
        `fieldValues` dictionary to access the contents of the field
        after calling `show()`.
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        User-friendly text label to place next to the field.
        :::

    -   ##### columns: [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        The values to display in the picker. Should be an array
        containing arrays of string values, each sub-array representing
        a column in the picker. Example two column picker:
        `[["Item 1", "Item 2"],["Column 2 Item 1", "Column 2 Item 2"]]`
        :::

    -   ##### selectedRows: [number]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        Array of zero-based index values to set the initial selected row
        in each column.
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-4 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addselect .tsd-anchor}

### addSelect

-   addSelect[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, values[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol},
    selectedValues[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol},
    allowMultiple[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:206](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L206)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a select control. Returns an array of string values in
    `fieldValues`.
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Identifier for the field. This will be used as the key in the
        `fieldValues` dictionary to access the contents of the field
        after calling `show()`.
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        User-friendly text label to place next to the field.
        :::

    -   ##### values: [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        The array of string values that will be available to select.
        :::

    -   ##### selectedValues: [string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        Array of string values that should be initially selected when
        the prompt is displayed. All values in this array should match
        values in the `values` array.
        :::

    -   ##### allowMultiple: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        If `false`, selecting a value will deselect all other values. If
        `true`, the user may select multiple items.
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-5 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addswitch .tsd-anchor}

### addSwitch

-   addSwitch[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type},
    initialValue[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:160](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L160)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add an on/off toggle switch. The `fieldValues` entry for this item
    will be a boolean indicating whether the switch was on.
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Identifier for the field. This will be used as the key in the
        `fieldValues` dictionary to access the contents of the field
        after calling `show()`.
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        User-friendly text label to place next to the field.
        :::

    -   ##### initialValue: [boolean]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        indicate if the switch should be on or off when initially
        displayed.
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-6 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addtextfield .tsd-anchor}

### addTextField

-   addTextField[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, initialText[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[?:
    ]{.tsd-signature-symbol}[{
    ]{.tsd-signature-symbol}autocapitalization[?:
    ]{.tsd-signature-symbol}[capitalizationTypes](../globals.html#capitalizationtypes){.tsd-signature-type}[;
    ]{.tsd-signature-symbol}autocorrect[?:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[;
    ]{.tsd-signature-symbol}keyboard[?:
    ]{.tsd-signature-symbol}[keyboardTypes](../globals.html#keyboardtypes){.tsd-signature-type}[;
    ]{.tsd-signature-symbol}placeholder[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[;
    ]{.tsd-signature-symbol}wantsFocus[?:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[
    }]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:98](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L98)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a text input field to the prompt
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Identifier for the field. This will be used as the key in the
        `fieldValues` dictionary to access the contents of the field
        after calling `show()`.
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        User-friendly text label to place next to the field.
        :::

    -   ##### initialText: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The initial text contents for the field.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} options: [{ ]{.tsd-signature-symbol}autocapitalization[?: ]{.tsd-signature-symbol}[capitalizationTypes](../globals.html#capitalizationtypes){.tsd-signature-type}[; ]{.tsd-signature-symbol}autocorrect[?: ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[; ]{.tsd-signature-symbol}keyboard[?: ]{.tsd-signature-symbol}[keyboardTypes](../globals.html#keyboardtypes){.tsd-signature-type}[; ]{.tsd-signature-symbol}placeholder[?: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[; ]{.tsd-signature-symbol}wantsFocus[?: ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[ }]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        A dictionary of options for configuring the text field.
        :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} autocapitalization[?: ]{.tsd-signature-symbol}[capitalizationTypes](../globals.html#capitalizationtypes){.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} autocorrect[?: ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            Should system autocorrect be enabled in field, Default: true
            :::
            :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} keyboard[?: ]{.tsd-signature-symbol}[keyboardTypes](../globals.html#keyboardtypes){.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} placeholder[?: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            Placeholder text to use when field is empty
            :::
            :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} wantsFocus[?: ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            If true, focus this field when prompt is displayed
            :::
            :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-7 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addtextview .tsd-anchor}

### addTextView

-   addTextView[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, initialText[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[?:
    ]{.tsd-signature-symbol}[{
    ]{.tsd-signature-symbol}autocapitalization[?:
    ]{.tsd-signature-symbol}[capitalizationTypes](../globals.html#capitalizationtypes){.tsd-signature-type}[;
    ]{.tsd-signature-symbol}autocorrect[?:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[;
    ]{.tsd-signature-symbol}height[?:
    ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[;
    ]{.tsd-signature-symbol}keyboard[?:
    ]{.tsd-signature-symbol}[keyboardTypes](../globals.html#keyboardtypes){.tsd-signature-type}[;
    ]{.tsd-signature-symbol}wantsFocus[?:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[
    }]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:128](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L128)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a text input field to the prompt
    :::
    :::

    #### Parameters {#parameters-8 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Identifier for the field. This will be used as the key in the
        `fieldValues` dictionary to access the contents of the field
        after calling `show()`.
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        User-friendly text label to place next to the field.
        :::

    -   ##### initialText: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The initial text contents for the field.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} options: [{ ]{.tsd-signature-symbol}autocapitalization[?: ]{.tsd-signature-symbol}[capitalizationTypes](../globals.html#capitalizationtypes){.tsd-signature-type}[; ]{.tsd-signature-symbol}autocorrect[?: ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[; ]{.tsd-signature-symbol}height[?: ]{.tsd-signature-symbol}[number]{.tsd-signature-type}[; ]{.tsd-signature-symbol}keyboard[?: ]{.tsd-signature-symbol}[keyboardTypes](../globals.html#keyboardtypes){.tsd-signature-type}[; ]{.tsd-signature-symbol}wantsFocus[?: ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}[ }]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        A dictionary of options for configuring the text field.
        :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} autocapitalization[?: ]{.tsd-signature-symbol}[capitalizationTypes](../globals.html#capitalizationtypes){.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} autocorrect[?: ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            Should system autocorrect be enabled in field, Default: true
            :::
            :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} height[?: ]{.tsd-signature-symbol}[number]{.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} keyboard[?: ]{.tsd-signature-symbol}[keyboardTypes](../globals.html#keyboardtypes){.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} wantsFocus[?: ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            If true, focus this field when prompt is displayed
            :::
            :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-8 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Other Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#show .tsd-anchor}

### show

-   show[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:226](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L226)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Displays the prompt. Returns `true` if the user selected one of the
    buttons in the buttons array, `false` if the user selected the
    \"Cancel\" button. After the dialog has been shown, the
    `buttonPressed` property will contain the name of the button
    selected by the user.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Prompt](prompt.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Prompt.d.ts:231](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Prompt.d.ts#L231)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [Prompt](prompt.html){.tsd-signature-type} {#returns-prompt-1 .tsd-returns-title}
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
-   [Prompt](prompt.html){.tsd-kind-icon}
    -   [constructor](prompt.html#constructor){.tsd-kind-icon}
    -   [buttonPressed](prompt.html#buttonpressed){.tsd-kind-icon}
    -   [fieldValues](prompt.html#fieldvalues){.tsd-kind-icon}
    -   [isCancellable](prompt.html#iscancellable){.tsd-kind-icon}
    -   [message](prompt.html#message){.tsd-kind-icon}
    -   [title](prompt.html#title){.tsd-kind-icon}
    -   [addButton](prompt.html#addbutton){.tsd-kind-icon}
    -   [addDatePicker](prompt.html#adddatepicker){.tsd-kind-icon}
    -   [addLabel](prompt.html#addlabel){.tsd-kind-icon}
    -   [addPasswordField](prompt.html#addpasswordfield){.tsd-kind-icon}
    -   [addPicker](prompt.html#addpicker){.tsd-kind-icon}
    -   [addSelect](prompt.html#addselect){.tsd-kind-icon}
    -   [addSwitch](prompt.html#addswitch){.tsd-kind-icon}
    -   [addTextField](prompt.html#addtextfield){.tsd-kind-icon}
    -   [addTextView](prompt.html#addtextview){.tsd-kind-icon}
    -   [show](prompt.html#show){.tsd-kind-icon}
    -   [create](prompt.html#create){.tsd-kind-icon}

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
