---
{"dg-publish":true,"permalink":"/snippets/outlookmessage/","dgHomeLink":true,"dgPassFrontmatter":false}
---

outlookmessage

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
-   [OutlookMessage](outlookmessage.html)

Class OutlookMessage
====================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#outlookmessage){#outlookmessage}

OutlookMessage
==============
:::

The OutlookMessage object can be used to create and send mail messages
through Outlook.com integrated accounts, similar to those created by a
[Outlook action step](https://getdrafts.com/actions/steps/outlook).
Creating and sending these messages happens in the background, with no
user interface, so messages must be complete with recipients before
calling `send()`. Sending is done via the [Microsoft Graph
API](https://developer.microsoft.com/en-us/graph). Outlooks accounts are
authenticated when used for the first time using OAuth - to use more
than one account, call create with different identifier parameters.

[](#example){#example}

### Example

    let message = OutlookMessage.create();
    message.toRecipients = ["joe@sample.com", "Jim Test <jim@test.com>"];
    message.subject = "My test message";
    message.body = "Body text";

    var success = message.send();
    if (!success) {
      console.log("Sending outlook message failed");
      context.fail();
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [OutlookMessage]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](outlookmessage.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [bccRecipients](outlookmessage.html#bccrecipients){.tsd-kind-icon}
-   [body](outlookmessage.html#body){.tsd-kind-icon}
-   [ccRecipients](outlookmessage.html#ccrecipients){.tsd-kind-icon}
-   [isBodyHTML](outlookmessage.html#isbodyhtml){.tsd-kind-icon}
-   [subject](outlookmessage.html#subject){.tsd-kind-icon}
-   [toRecipients](outlookmessage.html#torecipients){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [send](outlookmessage.html#send){.tsd-kind-icon}
-   [create](outlookmessage.html#create){.tsd-kind-icon}
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

-   new OutlookMessage[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[OutlookMessage](outlookmessage.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [OutlookMessage.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OutlookMessage.d.ts#L56)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [OutlookMessage](outlookmessage.html){.tsd-signature-type} {#returns-outlookmessage .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#bccrecipients .tsd-anchor}

### bccRecipients

::: {.tsd-signature .tsd-kind-icon}
bccRecipients[:]{.tsd-signature-symbol}
[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [OutlookMessage.d.ts:33](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OutlookMessage.d.ts#L33)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of email addresses to use as `BCC:` recipients. Each entry can be
a valid email address, or a name and email in the format `Name<email>`.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#body .tsd-anchor}

### body

::: {.tsd-signature .tsd-kind-icon}
body[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [OutlookMessage.d.ts:40](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OutlookMessage.d.ts#L40)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Body text of the mail message. Can be plain text or HTML if the
`isBodyHTML` property is set to `true`.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#ccrecipients .tsd-anchor}

### ccRecipients

::: {.tsd-signature .tsd-kind-icon}
ccRecipients[:]{.tsd-signature-symbol}
[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [OutlookMessage.d.ts:29](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OutlookMessage.d.ts#L29)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of email addresses to use as `CC:` recipients. Each entry can be a
valid email address, or a name and email in the format `Name<email>`.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#isbodyhtml .tsd-anchor}

### isBodyHTML

::: {.tsd-signature .tsd-kind-icon}
isBodyHTML[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [OutlookMessage.d.ts:45](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OutlookMessage.d.ts#L45)

::: {.tsd-comment .tsd-typography}
::: {.lead}
whether to treat the body string and plain text or HTML. When set to
`true`, the `body` property should be set to full valid HTML.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#subject .tsd-anchor}

### subject

::: {.tsd-signature .tsd-kind-icon}
subject[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [OutlookMessage.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OutlookMessage.d.ts#L35)
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#torecipients .tsd-anchor}

### toRecipients

::: {.tsd-signature .tsd-kind-icon}
toRecipients[:]{.tsd-signature-symbol}
[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [OutlookMessage.d.ts:25](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OutlookMessage.d.ts#L25)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of email addresses to use as `To:` recipients. Each entry can be a
valid email address, or a name and email in the format `Name<email>`.
:::
:::
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#send .tsd-anchor}

### send

-   send[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [OutlookMessage.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OutlookMessage.d.ts#L50)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Send the mail message via the Microsoft Graph API.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[OutlookMessage](outlookmessage.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [OutlookMessage.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/OutlookMessage.d.ts#L56)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    create a new object.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        notes which for Outlook account to use. This string is an
        arbitrary value, but we recommend using the email address you
        wish to associate with the script. Each unique identifier will
        be associated with its own
        [Credential](https://getdrafts.com/settings/credentials).
        :::

    #### Returns [OutlookMessage](outlookmessage.html){.tsd-signature-type} {#returns-outlookmessage-1 .tsd-returns-title}
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
-   [OutlookMessage](outlookmessage.html){.tsd-kind-icon}
    -   [constructor](outlookmessage.html#constructor){.tsd-kind-icon}
    -   [bccRecipients](outlookmessage.html#bccrecipients){.tsd-kind-icon}
    -   [body](outlookmessage.html#body){.tsd-kind-icon}
    -   [ccRecipients](outlookmessage.html#ccrecipients){.tsd-kind-icon}
    -   [isBodyHTML](outlookmessage.html#isbodyhtml){.tsd-kind-icon}
    -   [subject](outlookmessage.html#subject){.tsd-kind-icon}
    -   [toRecipients](outlookmessage.html#torecipients){.tsd-kind-icon}
    -   [send](outlookmessage.html#send){.tsd-kind-icon}
    -   [create](outlookmessage.html#create){.tsd-kind-icon}

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
