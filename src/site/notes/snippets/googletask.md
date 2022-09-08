---
{"dg-publish":true,"permalink":"/snippets/googletask/","dgHomeLink":true,"dgPassFrontmatter":false}
---

googletask

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
-   [GoogleTask](googletask.html)

Class GoogleTask
================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#googletask){#googletask}

GoogleTask
==========
:::

Script integration with [Google
Tasks](https://support.google.com/tasks/answer/7675772?co=GENIE.Platform%3DDesktop&hl=en).
This object handles OAuth authentication and request signing. The entire
[Google Tasks API](https://developers.google.com/tasks) can be used with
the `request` method, and convenience methods are provided for common
API endpoints to manage tasks and lists.

Working with the return values and parameters for these methods requires
an understanding of the JSON objects created and returned by the API, so
refer to type specifications in the [API
Reference](https://developers.google.com/tasks) for details on values
supported in task and lists. Specifically, review the supported
properties of the
[Task](https://developers.google.com/tasks/reference/rest/v1/tasks) and
[TaskList](https://developers.google.com/tasks/reference/rest/v1/tasklists)
objects to understand the values included in fetched objects, and to
make modifications.

If an convenince API calls fails, typically the result will be an
`undefined` value, and the `lastError` property will contains error
detail information for troubleshooting.

[](#example){#example}

### Example

See [Examples-Google Task]() action group in the [Drafts
Directory](https://actions.getdrafts.com/). It contains several example
scripted actions.

    // create GoogleTask object
    let gtask = GoogleTask.create();
    // create task in "Test" list
    let list = gtask.findList("Test");
    let t = {
        "title": "My Task",
        "notes": "My notes on this task"
    };
    let task = gtask.createTask(list, t);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [GoogleTask]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](googletask.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [lastError](googletask.html#lasterror){.tsd-kind-icon}
-   [lastResponse](googletask.html#lastresponse){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Lists Methods

-   [createList](googletask.html#createlist){.tsd-kind-icon}
-   [findList](googletask.html#findlist){.tsd-kind-icon}
-   [getLists](googletask.html#getlists){.tsd-kind-icon}

### Other Methods

-   [request](googletask.html#request){.tsd-kind-icon}
-   [create](googletask.html#create){.tsd-kind-icon}

### Tasks Methods

-   [createTask](googletask.html#createtask){.tsd-kind-icon}
-   [getTask](googletask.html#gettask){.tsd-kind-icon}
-   [getTasks](googletask.html#gettasks){.tsd-kind-icon}
-   [moveTask](googletask.html#movetask){.tsd-kind-icon}
-   [updateTask](googletask.html#updatetask){.tsd-kind-icon}
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

-   new GoogleTask[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[GoogleTask](googletask.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:116](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L116)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [GoogleTask](googletask.html){.tsd-signature-type} {#returns-googletask .tsd-returns-title}
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
    [GoogleTask.d.ts:44](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L44)

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
    [GoogleTask.d.ts:39](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L39)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function succeeds, this property will contain the last response
returned by the Google Tasks API. The JSON returned by the API will be
parsed to an object and placed in this property. Refer to [Google Tasks
API documentation](https://developers.google.com/tasks) for details on
the contents of this object based on call made.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Lists Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createlist .tsd-anchor}

### createList

-   createList[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[googleTaskList](../globals.html#googletasklist){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:63](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L63)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create list by name.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

    #### Returns [googleTaskList](../globals.html#googletasklist){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-googletasklist-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#findlist .tsd-anchor}

### findList

-   findList[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[googleTaskList](../globals.html#googletasklist){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L57)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get specific list by name. This is a convenience method which will
    fetch lists and return the first one found with a matching name.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

    #### Returns [googleTaskList](../globals.html#googletasklist){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-googletasklist-undefined-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getlists .tsd-anchor}

### getLists

-   getLists[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[googleTaskList](../globals.html#googletasklist){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:51](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L51)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get all lists. [API
    documentation](https://developers.google.com/tasks/reference/rest/v1/tasklists/list)
    :::
    :::

    #### Returns [googleTaskList](../globals.html#googletasklist){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-googletasklist-undefined-2 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Other Methods
-------------

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
        [GoogleTask.d.ts:99](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L99)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Execute a request against the [Google Task
    API](https://developers.google.com/tasks). For successful requests,
    the HTTPResponse object will contain an object or array or objects
    decoded from the JSON returned by the API as appropriate to the
    request made. Refer to API documentation for details about the
    expected parameters and responses. Drafts will handle wrapping the
    request in the appropriate OAuth authentication flow. Requests
    should only be made to endpoints in the Google Tasks API which
    require the `https://www.googleapis.com/auth/tasks` authentication
    scope.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

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
            The HTTP method, like \"GET\", \"POST\", \"PATCH\", etc.
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
            The full URL to the endpoint in the [Google Tasks
            API](https://developers.google.com/tasks).
            :::
            :::

    #### Returns [HTTPResponse](httpresponse.html){.tsd-signature-type} {#returns-httpresponse .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[GoogleTask](googletask.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:116](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L116)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new GoogleTask object.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional string value used to identify a To Do account.
        Typically this can be omitted if you only work with one Google
        Task account in Drafts. Each unique identifier used for To Do
        accounts will share credentials - across both action steps and
        scripts.
        :::

    #### Returns [GoogleTask](googletask.html){.tsd-signature-type} {#returns-googletask-1 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Tasks Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createtask .tsd-anchor}

### createTask

-   createTask[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[googleTaskList](../globals.html#googletasklist){.tsd-signature-type},
    task[:
    ]{.tsd-signature-symbol}[googleTask](../globals.html#googletask){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[googleTask](../globals.html#googletask){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:80](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L80)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new task in the specified list. Note that the API adds new
    tasks to the top of lists. [API
    documentation](https://developers.google.com/tasks/reference/rest/v1/tasks/insert)
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### list: [googleTaskList](../globals.html#googletasklist){.tsd-signature-type}

    -   ##### task: [googleTask](../globals.html#googletask){.tsd-signature-type}

    #### Returns [googleTask](../globals.html#googletask){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-googletask-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettask .tsd-anchor}

### getTask

-   getTask[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}, taskID[:
    ]{.tsd-signature-symbol}[String]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[googleTask](../globals.html#googletask){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:75](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L75)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get task a specific task by ID. [API
    documentation](https://developers.google.com/tasks/reference/rest/v1/tasks/list)
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### list: [object]{.tsd-signature-type}

    -   ##### taskID: [String]{.tsd-signature-type}

    #### Returns [googleTask](../globals.html#googletask){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-googletask-undefined-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettasks .tsd-anchor}

### getTasks

-   getTasks[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[googleTask](../globals.html#googletask){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:70](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L70)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get tasks in a list. [API
    documentation](https://developers.google.com/tasks/reference/rest/v1/tasks/list)
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### list: [object]{.tsd-signature-type}

    #### Returns [googleTask](../globals.html#googletask){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-googletask-undefined-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#movetask .tsd-anchor}

### moveTask

-   moveTask[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[googleTaskList](../globals.html#googletasklist){.tsd-signature-type},
    task[:
    ]{.tsd-signature-symbol}[googleTask](../globals.html#googletask){.tsd-signature-type},
    params[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:90](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L90)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Move an existing task. Parameters can include `parent` or `previous`
    values, which should be the taskID for other tasks in the same list.
    Use `parent` to make the task a sub-task of another task, and
    `previous` to place the task in order after the specified taskID.
    [API
    documentation](https://developers.google.com/tasks/reference/rest/v1/tasks/move)
    :::
    :::

    #### Parameters {#parameters-8 .tsd-parameters-title}

    -   ##### list: [googleTaskList](../globals.html#googletasklist){.tsd-signature-type}

    -   ##### task: [googleTask](../globals.html#googletask){.tsd-signature-type}

    -   ##### params: [object]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#updatetask .tsd-anchor}

### updateTask

-   updateTask[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[googleTaskList](../globals.html#googletasklist){.tsd-signature-type},
    task[:
    ]{.tsd-signature-symbol}[googleTask](../globals.html#googletask){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[googleTask](../globals.html#googletask){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GoogleTask.d.ts:85](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GoogleTask.d.ts#L85)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Update an existing task. Typical usage would be to modify the
    contents of a task returned by `getTask` or `getTasks` and sending
    the modified version as an update [API
    documentation](https://developers.google.com/tasks/reference/rest/v1/tasks/patch)
    :::
    :::

    #### Parameters {#parameters-9 .tsd-parameters-title}

    -   ##### list: [googleTaskList](../globals.html#googletasklist){.tsd-signature-type}

    -   ##### task: [googleTask](../globals.html#googletask){.tsd-signature-type}

    #### Returns [googleTask](../globals.html#googletask){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-googletask-undefined-3 .tsd-returns-title}
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
-   [GoogleTask](googletask.html){.tsd-kind-icon}
    -   [constructor](googletask.html#constructor){.tsd-kind-icon}
    -   [lastError](googletask.html#lasterror){.tsd-kind-icon}
    -   [lastResponse](googletask.html#lastresponse){.tsd-kind-icon}
    -   [createList](googletask.html#createlist){.tsd-kind-icon}
    -   [createTask](googletask.html#createtask){.tsd-kind-icon}
    -   [findList](googletask.html#findlist){.tsd-kind-icon}
    -   [getLists](googletask.html#getlists){.tsd-kind-icon}
    -   [getTask](googletask.html#gettask){.tsd-kind-icon}
    -   [getTasks](googletask.html#gettasks){.tsd-kind-icon}
    -   [moveTask](googletask.html#movetask){.tsd-kind-icon}
    -   [request](googletask.html#request){.tsd-kind-icon}
    -   [updateTask](googletask.html#updatetask){.tsd-kind-icon}
    -   [create](googletask.html#create){.tsd-kind-icon}

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
