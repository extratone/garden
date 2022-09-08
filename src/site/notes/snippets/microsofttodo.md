---
{"dg-publish":true,"permalink":"/snippets/microsofttodo/","dgHomeLink":true,"dgPassFrontmatter":false}
---

microsofttodo

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
-   [MicrosoftToDo](microsofttodo.html)

Class MicrosoftToDo
===================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#microsofttodo){#microsofttodo}

MicrosoftToDo
=============
:::

Script integration with [Microsoft To Do](http://todo.microsoft.com/).
This object handles OAuth authentication and request signing. The entire
[Microsoft To Do Graph
API](https://docs.microsoft.com/en-us/graph/api/resources/todo-overview?view=graph-rest-1.0)
can be used with the `request` method, and convenience methods are
provided for common API endpoints to manage tasks and lists.

Working with the return values and parameters for these methods requires
an understanding of the JSON objects created and returned by the API, so
refer to type specifications in the [API
Reference](https://docs.microsoft.com/en-us/graph/api/resources/todo-overview?view=graph-rest-1.0)
for details on values supported in task and lists. Specifically, review
the supported properties of the
[Task](https://docs.microsoft.com/en-us/graph/api/resources/todotask?view=graph-rest-1.0)
and
[TaskList](https://docs.microsoft.com/en-us/graph/api/resources/todotasklist?view=graph-rest-1.0)
objects to understand the values included in fetched objects, and to
make modifications.

If an API calls fails, typically the result will be an `undefined`
value, and the `lastError` property will contains error detail
information for troubleshooting.

[](#example){#example}

### Example

See [Examples-Microsoft To Do](https://actions.getdrafts.com/g/1m3)
action group in the [Drafts Directory](https://actions.getdrafts.com/).
It contains several example scripted actions.

    // create MicrosoftToDo object
    let todo = MicrosoftToDo.create();
    // create task in "Test" list
    let list = todo.findList("Test");
    // create task object, more properties available, see API docs
    let task = {
    "title": `Task Title`,
    "importance": "high",
    "body": {
    "content": "Notes for the task",
    "contentType": "text"
    };
    "dueDateTime": {
    "dateTime": Date.today().addDays(1).toISOString(),
    "timeZone": "UTC"
    }
    };
    let t = todo.createTask(list, task);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [MicrosoftToDo]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](microsofttodo.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [lastError](microsofttodo.html#lasterror){.tsd-kind-icon}
-   [lastResponse](microsofttodo.html#lastresponse){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Linked Resource Methods

-   [createLinkedResource](microsofttodo.html#createlinkedresource){.tsd-kind-icon}

### Lists Methods

-   [createList](microsofttodo.html#createlist){.tsd-kind-icon}
-   [findList](microsofttodo.html#findlist){.tsd-kind-icon}
-   [getLists](microsofttodo.html#getlists){.tsd-kind-icon}

### Other Methods

-   [request](microsofttodo.html#request){.tsd-kind-icon}
-   [create](microsofttodo.html#create){.tsd-kind-icon}

### Tasks Methods

-   [createTask](microsofttodo.html#createtask){.tsd-kind-icon}
-   [getTask](microsofttodo.html#gettask){.tsd-kind-icon}
-   [getTasks](microsofttodo.html#gettasks){.tsd-kind-icon}
-   [updateTask](microsofttodo.html#updatetask){.tsd-kind-icon}
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

-   new MicrosoftToDo[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[MicrosoftToDo](microsofttodo.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:131](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L131)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [MicrosoftToDo](microsofttodo.html){.tsd-signature-type} {#returns-microsofttodo .tsd-returns-title}
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
    [MicrosoftToDo.d.ts:58](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L58)

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
    [MicrosoftToDo.d.ts:53](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L53)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If a function succeeds, this property will contain the last response
returned by the To Do API. The JSON returned by the API will be parsed
to an object and placed in this property. Refer to [To Do API
documentation](https://docs.microsoft.com/en-us/graph/api/resources/todo-overview?view=graph-rest-1.0)
for details on the contents of this object based on call made.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Linked Resource Methods
-----------------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createlinkedresource .tsd-anchor}

### createLinkedResource

-   createLinkedResource[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type},
    task[:
    ]{.tsd-signature-symbol}[microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type},
    linkedResource[:
    ]{.tsd-signature-symbol}[microsoftToDoLinkedResource](../globals.html#microsofttodolinkedresource){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[microsoftToDoLinkedResource](../globals.html#microsofttodolinkedresource){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:105](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L105)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new linked resource for a task. A linked resource is a
    reference to content in an external system, such as a link back to a
    draft. [API
    documentation](https://docs.microsoft.com/en-us/graph/api/resources/linkedresource?view=graph-rest-1.0)
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### list: [microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}

    -   ##### task: [microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}

    -   ##### linkedResource: [microsoftToDoLinkedResource](../globals.html#microsofttodolinkedresource){.tsd-signature-type}

    #### Returns [microsoftToDoLinkedResource](../globals.html#microsofttodolinkedresource){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-microsofttodolinkedresource-undefined .tsd-returns-title}
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
    ]{.tsd-signature-symbol}[microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:77](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L77)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create list by name.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

    #### Returns [microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-microsofttodotasklist-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#findlist .tsd-anchor}

### findList

-   findList[(]{.tsd-signature-symbol}name[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:71](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L71)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get specific list by name. This is a convenience method which will
    fetch lists and return the first one found with a matching name.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### name: [string]{.tsd-signature-type}

    #### Returns [microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-microsofttodotasklist-undefined-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getlists .tsd-anchor}

### getLists

-   getLists[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:65](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L65)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get all lists. [API
    documentation](https://docs.microsoft.com/en-us/graph/api/todotasklist-list-tasks?view=graph-rest-1.0&tabs=http)
    :::
    :::

    #### Returns [microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-microsofttodotasklist-undefined-2 .tsd-returns-title}
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
        [MicrosoftToDo.d.ts:114](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L114)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Execute a request against the [Microsoft To Do
    API](https://docs.microsoft.com/en-us/graph/api/resources/todo-overview?view=graph-rest-1.0).
    For successful requests, the HTTPResponse object will contain an
    object or array or objects decoded from the JSON returned by the API
    as appropriate to the request made. Refer to API documentation for
    details about the expected parameters and responses. Drafts will
    handle wrapping the request in the appropriate OAuth authentication
    flow. Requests should only be made to endpoints in the Microsoft
    Graph API which require the `Task.ReadWrite` authentication scope.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

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
            The full URL to the endpoint in the [To Do
            API](https://docs.microsoft.com/en-us/graph/api/resources/todo-overview?view=graph-rest-1.0).
            :::
            :::

    #### Returns [HTTPResponse](httpresponse.html){.tsd-signature-type} {#returns-httpresponse .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[MicrosoftToDo](microsofttodo.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:131](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L131)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Creates a new MicrosoftToDo object.
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional string value used to identify a To Do account.
        Typically this can be omitted if you only work with one To Do
        account in Drafts. Each unique identifier used for To Do
        accounts will share credentials - across both action steps and
        scripts.
        :::

    #### Returns [MicrosoftToDo](microsofttodo.html){.tsd-signature-type} {#returns-microsofttodo-1 .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Tasks Methods
-------------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createtask .tsd-anchor}

### createTask

-   createTask[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type},
    task[:
    ]{.tsd-signature-symbol}[microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:94](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L94)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new task in the specified list. [API
    documentation](https://docs.microsoft.com/en-us/graph/api/todotasklist-post-tasks?view=graph-rest-1.0&tabs=http)
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### list: [microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}

    -   ##### task: [microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}

    #### Returns [microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-microsofttodotask-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettask .tsd-anchor}

### getTask

-   getTask[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type},
    taskID[:
    ]{.tsd-signature-symbol}[String]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:89](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L89)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get a specific task by ID. [API
    documentation](https://docs.microsoft.com/en-us/graph/api/todotask-get?view=graph-rest-1.0&tabs=http)
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### list: [microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}

    -   ##### taskID: [String]{.tsd-signature-type}

    #### Returns [microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-microsofttodotask-undefined-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettasks .tsd-anchor}

### getTasks

-   getTasks[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:84](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L84)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get tasks in a list. [API
    documentation](https://docs.microsoft.com/en-us/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http)
    :::
    :::

    #### Parameters {#parameters-8 .tsd-parameters-title}

    -   ##### list: [microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}

    #### Returns [microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-microsofttodotask-undefined-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#updatetask .tsd-anchor}

### updateTask

-   updateTask[(]{.tsd-signature-symbol}list[:
    ]{.tsd-signature-symbol}[microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type},
    task[:
    ]{.tsd-signature-symbol}[microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MicrosoftToDo.d.ts:99](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MicrosoftToDo.d.ts#L99)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Update an existing task. Typical usage would be to modify the
    contents of a task returned by `getTask` or `getTasks` and sending
    the modified version as an update [API
    documentation](https://docs.microsoft.com/en-us/graph/api/todotask-update?view=graph-rest-1.0&tabs=http)
    :::
    :::

    #### Parameters {#parameters-9 .tsd-parameters-title}

    -   ##### list: [microsoftToDoTaskList](../globals.html#microsofttodotasklist){.tsd-signature-type}

    -   ##### task: [microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}

    #### Returns [microsoftToDoTask](../globals.html#microsofttodotask){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-microsofttodotask-undefined-3 .tsd-returns-title}
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
-   [MicrosoftToDo](microsofttodo.html){.tsd-kind-icon}
    -   [constructor](microsofttodo.html#constructor){.tsd-kind-icon}
    -   [lastError](microsofttodo.html#lasterror){.tsd-kind-icon}
    -   [lastResponse](microsofttodo.html#lastresponse){.tsd-kind-icon}
    -   [createLinkedResource](microsofttodo.html#createlinkedresource){.tsd-kind-icon}
    -   [createList](microsofttodo.html#createlist){.tsd-kind-icon}
    -   [createTask](microsofttodo.html#createtask){.tsd-kind-icon}
    -   [findList](microsofttodo.html#findlist){.tsd-kind-icon}
    -   [getLists](microsofttodo.html#getlists){.tsd-kind-icon}
    -   [getTask](microsofttodo.html#gettask){.tsd-kind-icon}
    -   [getTasks](microsofttodo.html#gettasks){.tsd-kind-icon}
    -   [request](microsofttodo.html#request){.tsd-kind-icon}
    -   [updateTask](microsofttodo.html#updatetask){.tsd-kind-icon}
    -   [create](microsofttodo.html#create){.tsd-kind-icon}

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
