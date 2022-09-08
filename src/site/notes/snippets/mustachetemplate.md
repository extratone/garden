---
{"dg-publish":true,"permalink":"/snippets/mustachetemplate/","dgHomeLink":true,"dgPassFrontmatter":false}
---

mustachetemplate

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
-   [MustacheTemplate](mustachetemplate.html)

Class MustacheTemplate
======================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#mustachetemplate){#mustachetemplate}

MustacheTemplate
================
:::

See also:
[`Draft.processMustachTemplate`](/classes/draft#processmustachetemplate)
for rendering with Mustache similar to how those templates are rendered
in actions. The `MustacheTemplate` object is for rendering with your own
custom context.

The MustacheTemplate object support rendering of templates using the
[Mustache](https://en.wikipedia.org/wiki/Mustache_%28template_system%29)
template style.

Mustache templates offer advanced features for iterating over items,
creating conditional blocks of text and more. This is still a bit of an
experimental feature, please send feedback if you are finding edge cases
or are interested in more functionality in this area.

The object can be used in one of two ways, by passing a specific
template as a string and rendering it, or by passing a path to a
subdirectory of the `iCloud Drive/Drafts/Library/Templates` folder which
can contain more than one Mustache style templates (with file extension
`.mustache`), and then rendering them. The late method has the advantage
of supporting the use of partial templates in the same folder.

For details on using Mustache templates, we recommend reviewing
[tutorials](https://www.bersling.com/2017/09/22/the-ultimate-mustache-tutorial/).

[](#about-passing-data-to-templates){#about-passing-data-to-templates}

### About Passing Data to Templates

When rendering Mustache templates, you pass the template itself and a
data object which contains the values available to insert. The data
object should be a Javascript object with keys and values. Values can be
basic data types (numbers, strings, dates) and also arrays or nested
objects which can be iterated using conventions of the Mustache syntax.

[](#example){#example}

### Example

    // create template to loop over drafts
    let t = `Template Output:
    {{#drafts}}
    Draft: {{content}}
    {{#isFlagged}}Flagged!{{/isFlagged}}{{^isFlagged}}Not Flagged{{/isFlagged}}
    {{/drafts}}`;

    let d1 = Draft.create();
    d1.content = "First draft";
    d1.isFlagged = true;
    let d2 = Draft.create();
    d2.content = "Second draft";
    let drafts = [d1, d2];

    let data = {
      "drafts": drafts
    };

    let template = MustacheTemplate.createWithTemplate(t);
    let result = template.render(data);
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [MustacheTemplate]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [contentType](mustachetemplate.html#contenttype){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [createWithPath](mustachetemplate.html#createwithpath){.tsd-kind-icon}
-   [createWithTemplate](mustachetemplate.html#createwithtemplate){.tsd-kind-icon}
-   [render](mustachetemplate.html#render){.tsd-kind-icon}
-   [renderTemplate](mustachetemplate.html#rendertemplate){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#contenttype .tsd-anchor}

### contentType

::: {.tsd-signature .tsd-kind-icon}
contentType[:]{.tsd-signature-symbol} [\"text\"]{.tsd-signature-type}[
\| ]{.tsd-signature-symbol}[\"html\"]{.tsd-signature-type}
:::

-   Defined in
    [MustacheTemplate.d.ts:62](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MustacheTemplate.d.ts#L62)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Determines how the Mustache engine renders output. Valid options:

-   `text`: Render the output as plain text, do not do additional
    encoding of entities.
-   `html`: Render output as escaped HTML with entities converted for
    use in HTML.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createwithpath .tsd-anchor}

### createWithPath

-   createWithPath[(]{.tsd-signature-symbol}path[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[MustacheTemplate](mustachetemplate.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MustacheTemplate.d.ts:74](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MustacheTemplate.d.ts#L74)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a new object configured to point to a directory of Mustache
    template files in iCloud Drive. When using this method, other
    Mustache template located in the same directory will be available to
    be used as partials in the rendering process.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### path: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Relative path to a directory of Mustache template files (with
        .mustache file extension) located in
        `iCloud Drive/Drafts/Library/Templates`. For example to refer to
        templates in the directory
        `iCloud Drive/Drafts/Library/Templates/My Mustache Templates/`,
        pass `My Mustache Templates/` to this method.
        :::

    #### Returns [MustacheTemplate](mustachetemplate.html){.tsd-signature-type} {#returns-mustachetemplate .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#createwithtemplate .tsd-anchor}

### createWithTemplate

-   createWithTemplate[(]{.tsd-signature-symbol}template[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[MustacheTemplate](mustachetemplate.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MustacheTemplate.d.ts:68](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MustacheTemplate.d.ts#L68)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a new object with a template
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### template: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        a valid Mustache template string
        :::

    #### Returns [MustacheTemplate](mustachetemplate.html){.tsd-signature-type} {#returns-mustachetemplate-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#render .tsd-anchor}

### render

-   render[(]{.tsd-signature-symbol}data[:
    ]{.tsd-signature-symbol}[{}]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MustacheTemplate.d.ts:48](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MustacheTemplate.d.ts#L48)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Use in combination with `createWithTemplate(template)` to render the
    template using the data passsed.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### data: [{}]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        A Javascript object with the values to use when rendering the
        template. The object can have nested sub-objects.
        :::

        -   ##### [\[]{.tsd-signature-symbol}x: [string]{.tsd-signature-type}[\]: ]{.tsd-signature-symbol}[any]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type} {#returns-string .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#rendertemplate .tsd-anchor}

### renderTemplate

-   renderTemplate[(]{.tsd-signature-symbol}templateName[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, data[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [MustacheTemplate.d.ts:55](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/MustacheTemplate.d.ts#L55)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Use in combination with `createWithPath(path)` to render the
    template using the data passsed.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### templateName: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The name of a template file in the directory passed to create
        the MustacheTemplate object. Do not include the \".mustache\"
        file extension. For example, if you have a \"Document.mustache\"
        file in the directory, pass templateName \"Document\".
        :::

    -   ##### data: [any]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        A Javascript object with the values to use when rendering the
        template. The object can have nested sub-objects.
        :::

    #### Returns [string]{.tsd-signature-type} {#returns-string-1 .tsd-returns-title}
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
-   [MustacheTemplate](mustachetemplate.html){.tsd-kind-icon}
    -   [contentType](mustachetemplate.html#contenttype){.tsd-kind-icon}
    -   [createWithPath](mustachetemplate.html#createwithpath){.tsd-kind-icon}
    -   [createWithTemplate](mustachetemplate.html#createwithtemplate){.tsd-kind-icon}
    -   [render](mustachetemplate.html#render){.tsd-kind-icon}
    -   [renderTemplate](mustachetemplate.html#rendertemplate){.tsd-kind-icon}

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
