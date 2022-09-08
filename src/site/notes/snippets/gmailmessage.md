---
{"dg-publish":true,"permalink":"/snippets/gmailmessage/","dgHomeLink":true,"dgPassFrontmatter":false}
---

gmailmessage

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
-   [GmailMessage](gmailmessage.html)

Class GmailMessage
==================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#gmailmessage){#gmailmessage}

GmailMessage
============
:::

The GmailMessage object can be used to create and send mail messages
through Gmail accounts, similar to those created by a [Gmail action
step](https://getdrafts.com/actions/steps/gmail). Creating and sending
these messages happens in the background, with no user interface, so
messages must be complete with recipients before calling send(). Sending
is done via the [Gmail API](https://developers.google.com/gmail/api/).
Gmail accounts are authenticated when used for the first time using
OAuth - to use more than one account, call create with different
identifier parameters.

[](#example){#example}

### Example

    let message = GmailMessage.create();
    message.toRecipients = ["joe@sample.com"];
    message.subject = "My test message";
    message.body = "Body text";

    var success = message.send();
    if (!success) {
      console.log("Sending gmail failed");
      context.fail();
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [GmailMessage]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](gmailmessage.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [bccRecipients](gmailmessage.html#bccrecipients){.tsd-kind-icon}
-   [body](gmailmessage.html#body){.tsd-kind-icon}
-   [ccRecipients](gmailmessage.html#ccrecipients){.tsd-kind-icon}
-   [isBodyHTML](gmailmessage.html#isbodyhtml){.tsd-kind-icon}
-   [subject](gmailmessage.html#subject){.tsd-kind-icon}
-   [toRecipients](gmailmessage.html#torecipients){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [send](gmailmessage.html#send){.tsd-kind-icon}
-   [create](gmailmessage.html#create){.tsd-kind-icon}
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

-   new GmailMessage[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[GmailMessage](gmailmessage.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GmailMessage.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GmailMessage.d.ts#L56)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

    #### Returns [GmailMessage](gmailmessage.html){.tsd-signature-type} {#returns-gmailmessage .tsd-returns-title}
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
    [GmailMessage.d.ts:33](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GmailMessage.d.ts#L33)

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
    [GmailMessage.d.ts:40](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GmailMessage.d.ts#L40)

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
    [GmailMessage.d.ts:29](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GmailMessage.d.ts#L29)

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
    [GmailMessage.d.ts:45](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GmailMessage.d.ts#L45)

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
    [GmailMessage.d.ts:35](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GmailMessage.d.ts#L35)
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#torecipients .tsd-anchor}

### toRecipients

::: {.tsd-signature .tsd-kind-icon}
toRecipients[:]{.tsd-signature-symbol}
[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [GmailMessage.d.ts:25](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GmailMessage.d.ts#L25)

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
        [GmailMessage.d.ts:50](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GmailMessage.d.ts#L50)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Send the mail message via the Gmail API.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[GmailMessage](gmailmessage.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [GmailMessage.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/GmailMessage.d.ts#L56)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    create a new object.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        notes which for Gmail account to use. This string is an
        arbitrary value, but we recommend using the email address you
        wish to associate with the script. Each unique identifier will
        be associated with its own
        [Credential](https://getdrafts.com/settings/credentials).
        :::

    #### Returns [GmailMessage](gmailmessage.html){.tsd-signature-type} {#returns-gmailmessage-1 .tsd-returns-title}
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
-   [GmailMessage](gmailmessage.html){.tsd-kind-icon}
    -   [constructor](gmailmessage.html#constructor){.tsd-kind-icon}
    -   [bccRecipients](gmailmessage.html#bccrecipients){.tsd-kind-icon}
    -   [body](gmailmessage.html#body){.tsd-kind-icon}
    -   [ccRecipients](gmailmessage.html#ccrecipients){.tsd-kind-icon}
    -   [isBodyHTML](gmailmessage.html#isbodyhtml){.tsd-kind-icon}
    -   [subject](gmailmessage.html#subject){.tsd-kind-icon}
    -   [toRecipients](gmailmessage.html#torecipients){.tsd-kind-icon}
    -   [send](gmailmessage.html#send){.tsd-kind-icon}
    -   [create](gmailmessage.html#create){.tsd-kind-icon}

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
