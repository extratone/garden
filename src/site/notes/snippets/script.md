---
{"dg-publish":true,"permalink":"/snippets/script/","dgHomeLink":true,"dgPassFrontmatter":false}
---

script

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
-   [Script](script.html)

Class Script
============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#script){#script}

Script
======
:::

When running a [Script action
step](https://docs.getdrafts.com/docs/actions/steps/advanced.html#script),
a single `script` object will be in context to reference the currently
running script.

[](#example){#example}

### Example

    function sleep(milliseconds) {
      var start = new Date().getTime();
      for (var i = 0; i < 1e7; i++) {
        if ((new Date().getTime() - start) > milliseconds){
          break;
        }
      }
    }
    async function f() {
      let promise = new Promise((resolve, reject) => {
        sleep(1000);
        resolve("done!")
      });
      let result = await promise; // wait until the promise resolves (*)
      alert(result); // "done!"
      script.complete();
    }
    f();
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Script]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Methods

-   [complete](script.html#complete){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#complete .tsd-anchor}

### complete

-   complete[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Script.d.ts:32](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Script.d.ts#L32)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Inform Drafts the current script has completed execution. Used in
    combination with the \"Allow asynchronous execution\" option of the
    Script step type. If your script step has the asynchronous option
    enabled, you *must* call `script.complete()` to indicate completion
    or the script will timeout and fail.
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
-   [Script](script.html){.tsd-kind-icon}
    -   [complete](script.html#complete){.tsd-kind-icon}

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
