---
{"dg-publish":true,"permalink":"/snippets/tjscontainer/","dgHomeLink":true,"dgPassFrontmatter":false}
---

tjscontainer

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
-   [TJSContainer](tjscontainer.html)

Class TJSContainer
==================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#tjscontainer){#tjscontainer}

TJSContainer
============
:::

Wraps an array of todo and/or project items and encodes them into a URL
for use to send the request to Things.

[](#things-integration-notes){#things-integration-notes}

Things Integration Notes
------------------------

-   [Things](https://culturedcode.com/things/) is a popular task and
    project management app from Cultured Code. Things supports advanced
    URL schemes (required Things v3.4 or greater on iOS) which can
    accept multiple todos, projects, headings in a single call to the
    app. The scripting interfaces below are convenience wrappers that
    allow easy creation and encoding of the URLs needed to pass this
    type of information to Things.

The TJS\* JavaScript objects are wrappers around an [open source Swift
library](https://github.com/culturedcode/ThingsJSONCoder) provided by
Cultured Code, with a few modifications to work in JavaScript. In all
cases, nothing is committed to Things until the the items are wrapped in
a TJSContainer, and the URL it generates called to send the data to
Things. This is best done with Drafts' `CallbackURL` object (see example
below).

For more information about what values Things understands in these
objects, refer to [their URL scheme
documenation](https://support.culturedcode.com/customer/en/portal/articles/2803573).

[](#example){#example}

### Example

    // create a Things Project
    var project = TJSProject.create();
    project.title = "My Project From Drafts";
    project.notes = "Let's do this stuff";

    // create and add a heading to the project
    var heading = TJSHeading.create();
    heading.title = "First Heading";
    project.addHeading(heading);

    // add todos to the project
    var todo1 = TJSTodo.create();
    todo1.title = "My first todo";
    todo1.when = "today";
    project.addTodo(todo1);

    var todo2 = TJSTodo.create();
    todo2.title = "My second todo";
    todo2.when = "tomorrow";
    project.addTodo(todo2);

    // create a container to handle creation of Things URL
    var container = TJSContainer.create([project]);

    // Use CallbackURL object to open URL in Things.
    var cb = CallbackURL.create();
    cb.baseURL = container.url;
    var success = cb.open();
    if (success) {
        console.log("Project created in Things");
    }
    else {
        context.fail();
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [TJSContainer]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [url](tjscontainer.html#url){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [create](tjscontainer.html#create){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#url .tsd-anchor}

### url

::: {.tsd-signature .tsd-kind-icon}
url[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Things.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Things.d.ts#L64)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The full URL with encoded TJSContainer parameters.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}items[:
    ]{.tsd-signature-symbol}[Array]{.tsd-signature-type}[\<]{.tsd-signature-symbol}[TJSProject](tjsproject.html){.tsd-signature-type}[
    \|
    ]{.tsd-signature-symbol}[TJSTodo](tjstodo.html){.tsd-signature-type}[\>]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[TJSContainer](tjscontainer.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Things.d.ts:60](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Things.d.ts#L60)

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### items: [Array]{.tsd-signature-type}[\<]{.tsd-signature-symbol}[TJSProject](tjsproject.html){.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[TJSTodo](tjstodo.html){.tsd-signature-type}[\>]{.tsd-signature-symbol}

    #### Returns [TJSContainer](tjscontainer.html){.tsd-signature-type} {#returns-tjscontainer .tsd-returns-title}
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
-   [TJSContainer](tjscontainer.html){.tsd-kind-icon}
    -   [url](tjscontainer.html#url){.tsd-kind-icon}
    -   [create](tjscontainer.html#create){.tsd-kind-icon}

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
