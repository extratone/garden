---
{"dg-publish":true,"permalink":"/snippets/version/","dgHomeLink":true,"dgPassFrontmatter":false}
---

version

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
-   [Version](version.html)

Class Version
=============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#version){#version}

Version
=======
:::

Version objects represent individual versions in a draft\'s [version
history](https://docs.getdrafts.com/docs/drafts/versionhistory).
Versions are accessed using the `versions` property of the
[Draft](draft.html) object.

    // loop over versions of a draft, keeping only most recent 3
    if (draft.versions.length > 3) {
      let versions = draft.versions.slice(3);
      for (let version of versions) {
        version.delete();
      }
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Version]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Properties

-   [content](version.html#content){.tsd-kind-icon}
-   [createdAt](version.html#createdat){.tsd-kind-icon}
-   [draft](version.html#draft){.tsd-kind-icon}
-   [uuid](version.html#uuid){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [delete](version.html#delete){.tsd-kind-icon}
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#content .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} content

::: {.tsd-signature .tsd-kind-icon}
content[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Version.d.ts:23](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Version.d.ts#L23)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The content of the draft at the time this version was saved
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#createdat .tsd-anchor}

### [Readonly]{.tsd-flag .ts-flagReadonly} createdAt

::: {.tsd-signature .tsd-kind-icon}
createdAt[:]{.tsd-signature-symbol} [Date]{.tsd-signature-type}
:::

-   Defined in
    [Version.d.ts:27](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Version.d.ts#L27)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Timestamp for the creation of the version
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#draft .tsd-anchor}

### [Optional]{.tsd-flag .ts-flagOptional} [Readonly]{.tsd-flag .ts-flagReadonly} draft

::: {.tsd-signature .tsd-kind-icon}
draft[:]{.tsd-signature-symbol} [Draft](draft.html){.tsd-signature-type}
:::

-   Defined in
    [Version.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Version.d.ts#L35)

::: {.tsd-comment .tsd-typography}
::: {.lead}
The [Draft](draft.html) object related to the version. Typically not
needed, as versions are accessed through the `versions` property of a
draft.
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
    [Version.d.ts:19](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Version.d.ts#L19)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Unique identifier of this version
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#delete .tsd-anchor}

### delete

-   delete[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Version.d.ts:31](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Version.d.ts#L31)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Delete the version. This is permanent and should be used with
    caution
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
-   [Version](version.html){.tsd-kind-icon}
    -   [content](version.html#content){.tsd-kind-icon}
    -   [createdAt](version.html#createdat){.tsd-kind-icon}
    -   [draft](version.html#draft){.tsd-kind-icon}
    -   [uuid](version.html#uuid){.tsd-kind-icon}
    -   [delete](version.html#delete){.tsd-kind-icon}

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
