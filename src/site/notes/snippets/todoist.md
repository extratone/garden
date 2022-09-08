---
{"dg-publish":true,"permalink":"/snippets/todoist/","dgHomeLink":true,"dgPassFrontmatter":false}
---

todoist

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
-   [Todoist](todoist.html)

Class Todoist
=============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#todoist){#todoist}

Todoist
=======
:::

Script integration with [Todoist](http://todoist.com/). This object
handles OAuth authentication and request signing. The entire [Todoist
REST API](https://developer.todoist.com/rest/v1/) can be used with the
request method, and convenience methods are provided for common API
endpoints to manage tasks, projects, comments and labels.

The `quickAdd` method is mostly likely what you are looking for to
create tasks as it supports the shorthand the task entry box in Todoist
supports to parse projects, etc.

Other methods are direct mappings of the REST API calls provided by
Todoist. Most take an `options` parameter which is a javascript object
containing the parameters to be passed to the API, and and the method
decodes the JSON response from Todoist and returns it as a Javascript
object (or array of objects) with the values as specified in the Todoist
API docs.

If an API calls fails, typically the result will be an `undefined`
value, and the `lastError` property will contains error detail
information for troubleshooting.

[](#example){#example}

### Example

See [Examples-Todoist](https://actions.getdrafts.com/g/1L3) action group
in the [Action Directory](https://actions.getdrafts.com/).

    // create Todoist object
    let todoist = Todoist.create();
    // create task in inbox
    todoist.createTask({
      "content": "My Task Name",
      "due_string": "Next wednesday"
    });
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Todoist]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](todoist.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [lastError](todoist.html#lasterror){.tsd-kind-icon}
-   [lastResponse](todoist.html#lastresponse){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Comments Methods

-   [createComment](todoist.html#createcomment){.tsd-kind-icon}
-   [getComment](todoist.html#getcomment){.tsd-kind-icon}
-   [getComments](todoist.html#getcomments){.tsd-kind-icon}
-   [updateComment](todoist.html#updatecomment){.tsd-kind-icon}

### Labels Methods

-   [createLabel](todoist.html#createlabel){.tsd-kind-icon}
-   [getLabel](todoist.html#getlabel){.tsd-kind-icon}
-   [getLabels](todoist.html#getlabels){.tsd-kind-icon}
-   [updateLabel](todoist.html#updatelabel){.tsd-kind-icon}

### Other Methods

-   [quickAdd](todoist.html#quickadd){.tsd-kind-icon}
-   [request](todoist.html#request){.tsd-kind-icon}
-   [create](todoist.html#create){.tsd-kind-icon}

### Projects Methods

-   [createProject](todoist.html#createproject){.tsd-kind-icon}
-   [getProject](todoist.html#getproject){.tsd-kind-icon}
-   [getProjects](todoist.html#getprojects){.tsd-kind-icon}
-   [updateProject](todoist.html#updateproject){.tsd-kind-icon}

### Sections Methods

-   [createSection](todoist.html#createsection){.tsd-kind-icon}
-   [getProjectSections](todoist.html#getprojectsections){.tsd-kind-icon}
-   [getSection](todoist.html#getsection){.tsd-kind-icon}
-   [getSections](todoist.html#getsections){.tsd-kind-icon}
-   [updateSection](todoist.html#updatesection){.tsd-kind-icon}

### Tasks Methods

-   [closeTask](todoist.html#closetask){.tsd-kind-icon}
-   [createTask](todoist.html#createtask){.tsd-kind-icon}
-   [getTask](todoist.html#gettask){.tsd-kind-icon}
-   [getTasks](todoist.html#gettasks){.tsd-kind-icon}
-   [reopenTask](todoist.html#reopentask){.tsd-kind-icon}
-   [updateTask](todoist.html#updatetask){.tsd-kind-icon}
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

-   new Todoist[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Todoist](todoist.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:194](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L194)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [Todoist](todoist.html){.tsd-signature-type} {#returns-todoist .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lasterror .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} lastError

::: {.tsd-signature .tsd-kind-icon}
lastError[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Todoist.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L35)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function fails, this property will contain the last error as a
string message, otherwise it will be `undefined`.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#lastresponse .tsd-anchor}

### lastResponse

::: {.tsd-signature .tsd-kind-icon}
lastResponse[:]{.tsd-signature-symbol} [any]{.tsd-signature-type}
:::

-   Defined in
    [Todoist.d.ts:30](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L30)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function succeeds, this property will contain the last response
returned by Todoist. The JSON returned by Todoist will be parsed to an
object and placed in this property. Refer to [Todoist API
documentation](https://developer.todoist.com/rest/v8) for details on the
contents of this object based on call made.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Comments Methods
----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createcomment .tsd-anchor}

### createComment

-   createComment[(]{.tsd-signature-symbol}options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:137](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L137)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new comment. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#create-a-new-comment)
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getcomment .tsd-anchor}

### getComment

-   getComment[(]{.tsd-signature-symbol}commentId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:142](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L142)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get comment. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-a-comment)
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### commentId: [string]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getcomments .tsd-anchor}

### getComments

-   getComments[(]{.tsd-signature-symbol}options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:132](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L132)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get all comments. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-all-comments)
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-object-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#updatecomment .tsd-anchor}

### updateComment

-   updateComment[(]{.tsd-signature-symbol}commentId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:147](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L147)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Update comment. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#update-a-comment)
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### commentId: [string]{.tsd-signature-type}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-3 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Labels Methods
--------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createlabel .tsd-anchor}

### createLabel

-   createLabel[(]{.tsd-signature-symbol}options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:159](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L159)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new labels. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#create-a-new-label)
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-4 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getlabel .tsd-anchor}

### getLabel

-   getLabel[(]{.tsd-signature-symbol}labelId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:164](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L164)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get label. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-a-label)
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### labelId: [string]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-5 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getlabels .tsd-anchor}

### getLabels

-   getLabels[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:154](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L154)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get all labels. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-all-labels)
    :::
    :::

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-object-6 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#updatelabel .tsd-anchor}

### updateLabel

-   updateLabel[(]{.tsd-signature-symbol}labelId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:169](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L169)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Update label. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#update-a-label)
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### labelId: [string]{.tsd-signature-type}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-7 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Other Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#quickadd .tsd-anchor}

### quickAdd

-   quickAdd[(]{.tsd-signature-symbol}text[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, note[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, reminder[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[?:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:44](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L44)

    ::: {.tsd-comment .tsd-typography}
    :::

    #### Parameters {#parameters-8 .tsd-parameters-title}

    -   ##### text: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Text to use to create the task. Supports Todoist quick add
        notation for specifying projects, priority, labels, etc. just as
        if you were using the Todoist quick add window.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} note: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional text to attach as a comment with the task.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} reminder: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional natural language date specifying for creating a task
        reminder.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} options: [object]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional dictionary of additional parameters to include in the
        request.
        :::

    #### Returns [object]{.tsd-signature-type} {#returns-object-8 .tsd-returns-title}

    Object containing respose data from Todoist.
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#request .tsd-anchor}

### request

-   request[(]{.tsd-signature-symbol}settings[:
    ]{.tsd-signature-symbol}[{ ]{.tsd-signature-symbol}data[?:
    ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[;
    ]{.tsd-signature-symbol}headers[?:
    ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[;
    ]{.tsd-signature-symbol}method[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[;
    ]{.tsd-signature-symbol}parameters[?:
    ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[;
    ]{.tsd-signature-symbol}url[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[
    }]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[HTTPResponse](httpresponse.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:177](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L177)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Execute a request against the Todoist API. For successful requests,
    the HTTPResponse object will contain an object or array or objects
    decoded from the JSON returned by Todoist as appropriate to the
    request made. Refer to Todoist's API documentation for details about
    the expected parameters and responses. Drafts will handle wrapping
    the request in the appropriate OAuth authentication flow.
    :::
    :::

    #### Parameters {#parameters-9 .tsd-parameters-title}

    -   ##### settings: [{ ]{.tsd-signature-symbol}data[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}headers[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}method[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[; ]{.tsd-signature-symbol}parameters[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[; ]{.tsd-signature-symbol}url[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[ }]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        an object configuring the request.
        :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} data[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            A JavaScript object containing data to be encoded into the
            HTTP body of the request.
            :::
            :::

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} headers[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            An object contain key-values to be added as custom headers
            in the request. There is no need to provide authorization
            headers, Drafts will add those.
            :::
            :::

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### method[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            The HTTP method, like \"GET\", \"POST\", etc.
            :::
            :::

        -   ##### [Optional]{.tsd-flag .ts-flagOptional} parameters[?: ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            An object containing key-values to be added to the request
            as URL parameters.
            :::
            :::

            -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

        -   ##### url[: ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

            ::: {.tsd-comment .tsd-typography}
            ::: {.lead}
            The full URL to the endpoint in the [Todoist REST
            API](https://developer.todoist.com/rest/v1/).
            :::
            :::

    #### Returns [HTTPResponse](httpresponse.html){.tsd-signature-type} {#returns-httpresponse .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Todoist](todoist.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:194](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L194)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new Todoist object.
    :::
    :::

    #### Parameters {#parameters-10 .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional string value used to identify a Todoist account.
        Typically this can be omitted if you only work with one Todoist
        account in Drafts. Each unique identifier used for Todoist
        accounts will share credentials - across both action steps and
        scripts.
        :::

    #### Returns [Todoist](todoist.html){.tsd-signature-type} {#returns-todoist-1 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Projects Methods
----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createproject .tsd-anchor}

### createProject

-   createProject[(]{.tsd-signature-symbol}options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:88](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L88)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new project. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#create-a-new-project)
    :::
    :::

    #### Parameters {#parameters-11 .tsd-parameters-title}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-9 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getproject .tsd-anchor}

### getProject

-   getProject[(]{.tsd-signature-symbol}projectId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:93](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L93)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get project. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-a-project)
    :::
    :::

    #### Parameters {#parameters-12 .tsd-parameters-title}

    -   ##### projectId: [string]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-10 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getprojects .tsd-anchor}

### getProjects

-   getProjects[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:83](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L83)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get all projects. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-all-projects)
    :::
    :::

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-object-11 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#updateproject .tsd-anchor}

### updateProject

-   updateProject[(]{.tsd-signature-symbol}projectId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:98](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L98)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Update project. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#update-a-project)
    :::
    :::

    #### Parameters {#parameters-13 .tsd-parameters-title}

    -   ##### projectId: [string]{.tsd-signature-type}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-12 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Sections Methods
----------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createsection .tsd-anchor}

### createSection

-   createSection[(]{.tsd-signature-symbol}options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:115](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L115)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new section. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#create-a-new-section)
    :::
    :::

    #### Parameters {#parameters-14 .tsd-parameters-title}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-13 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getprojectsections .tsd-anchor}

### getProjectSections

-   getProjectSections[(]{.tsd-signature-symbol}projectId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:110](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L110)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get project sections. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-project-sections)
    :::
    :::

    #### Parameters {#parameters-15 .tsd-parameters-title}

    -   ##### projectId: [string]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-object-14 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getsection .tsd-anchor}

### getSection

-   getSection[(]{.tsd-signature-symbol}sectionId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:120](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L120)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get section. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-a-single-section)
    :::
    :::

    #### Parameters {#parameters-16 .tsd-parameters-title}

    -   ##### sectionId: [string]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-15 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getsections .tsd-anchor}

### getSections

-   getSections[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:105](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L105)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get all sections. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-all-sections)
    :::
    :::

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-object-16 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#updatesection .tsd-anchor}

### updateSection

-   updateSection[(]{.tsd-signature-symbol}sectionId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:125](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L125)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Update section. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#update-a-section)
    :::
    :::

    #### Parameters {#parameters-17 .tsd-parameters-title}

    -   ##### sectionId: [string]{.tsd-signature-type}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-17 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Tasks Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#closetask .tsd-anchor}

### closeTask

-   closeTask[(]{.tsd-signature-symbol}taskId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:71](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L71)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Close task (mark complete)
    :::
    :::

    #### Parameters {#parameters-18 .tsd-parameters-title}

    -   ##### taskId: [string]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createtask .tsd-anchor}

### createTask

-   createTask[(]{.tsd-signature-symbol}options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L56)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new task. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#create-a-new-task)
    :::
    :::

    #### Parameters {#parameters-19 .tsd-parameters-title}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-18 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettask .tsd-anchor}

### getTask

-   getTask[(]{.tsd-signature-symbol}taskId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:61](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L61)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get active task. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-an-active-task)
    :::
    :::

    #### Parameters {#parameters-20 .tsd-parameters-title}

    -   ##### taskId: [string]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-19 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettasks .tsd-anchor}

### getTasks

-   getTasks[(]{.tsd-signature-symbol}options[?:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:51](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L51)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get active tasks. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#get-active-tasks)
    :::
    :::

    #### Parameters {#parameters-21 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol} {#returns-object-20 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#reopentask .tsd-anchor}

### reopenTask

-   reopenTask[(]{.tsd-signature-symbol}taskId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:76](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L76)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Reopen task (mark incomplete)
    :::
    :::

    #### Parameters {#parameters-22 .tsd-parameters-title}

    -   ##### taskId: [string]{.tsd-signature-type}

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#updatetask .tsd-anchor}

### updateTask

-   updateTask[(]{.tsd-signature-symbol}taskId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, options[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Todoist.d.ts:66](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Todoist.d.ts#L66)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Update active task. [Todoist API
    documentation](https://developer.todoist.com/rest/v1/#update-a-task)
    :::
    :::

    #### Parameters {#parameters-23 .tsd-parameters-title}

    -   ##### taskId: [string]{.tsd-signature-type}

    -   ##### options: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type} {#returns-object-21 .tsd-returns-title}
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
-   [Todoist](todoist.html){.tsd-kind-icon}
    -   [constructor](todoist.html#constructor){.tsd-kind-icon}
    -   [lastError](todoist.html#lasterror){.tsd-kind-icon}
    -   [lastResponse](todoist.html#lastresponse){.tsd-kind-icon}
    -   [closeTask](todoist.html#closetask){.tsd-kind-icon}
    -   [createComment](todoist.html#createcomment){.tsd-kind-icon}
    -   [createLabel](todoist.html#createlabel){.tsd-kind-icon}
    -   [createProject](todoist.html#createproject){.tsd-kind-icon}
    -   [createSection](todoist.html#createsection){.tsd-kind-icon}
    -   [createTask](todoist.html#createtask){.tsd-kind-icon}
    -   [getComment](todoist.html#getcomment){.tsd-kind-icon}
    -   [getComments](todoist.html#getcomments){.tsd-kind-icon}
    -   [getLabel](todoist.html#getlabel){.tsd-kind-icon}
    -   [getLabels](todoist.html#getlabels){.tsd-kind-icon}
    -   [getProject](todoist.html#getproject){.tsd-kind-icon}
    -   [getProjectSections](todoist.html#getprojectsections){.tsd-kind-icon}
    -   [getProjects](todoist.html#getprojects){.tsd-kind-icon}
    -   [getSection](todoist.html#getsection){.tsd-kind-icon}
    -   [getSections](todoist.html#getsections){.tsd-kind-icon}
    -   [getTask](todoist.html#gettask){.tsd-kind-icon}
    -   [getTasks](todoist.html#gettasks){.tsd-kind-icon}
    -   [quickAdd](todoist.html#quickadd){.tsd-kind-icon}
    -   [reopenTask](todoist.html#reopentask){.tsd-kind-icon}
    -   [request](todoist.html#request){.tsd-kind-icon}
    -   [updateComment](todoist.html#updatecomment){.tsd-kind-icon}
    -   [updateLabel](todoist.html#updatelabel){.tsd-kind-icon}
    -   [updateProject](todoist.html#updateproject){.tsd-kind-icon}
    -   [updateSection](todoist.html#updatesection){.tsd-kind-icon}
    -   [updateTask](todoist.html#updatetask){.tsd-kind-icon}
    -   [create](todoist.html#create){.tsd-kind-icon}

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
