---
{"dg-publish":true,"permalink":"/snippets/mail/","dgHomeLink":true,"dgPassFrontmatter":false}
---

mail

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
-   [Mail](mail.html)

Class Mail
==========
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Mail]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](mail.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [bccRecipients](mail.html#bccrecipients){.tsd-kind-icon}
-   [body](mail.html#body){.tsd-kind-icon}
-   [ccRecipients](mail.html#ccrecipients){.tsd-kind-icon}
-   [isBodyHTML](mail.html#isbodyhtml){.tsd-kind-icon}
-   [isSent](mail.html#issent){.tsd-kind-icon}
-   [sendInBackground](mail.html#sendinbackground){.tsd-kind-icon}
-   [status](mail.html#status){.tsd-kind-icon}
-   [subject](mail.html#subject){.tsd-kind-icon}
-   [toRecipients](mail.html#torecipients){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [send](mail.html#send){.tsd-kind-icon}
-   [create](mail.html#create){.tsd-kind-icon}
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

-   new Mail[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Mail](mail.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Mail.d.ts:95](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L95)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [Mail](mail.html){.tsd-signature-type} {#returns-mail .tsd-returns-title}
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
    [Mail.d.ts:47](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L47)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of email addresses to use as `BCC:` recipients.
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
    [Mail.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L57)

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
    [Mail.d.ts:42](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L42)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of email addresses to use as `CC:` recipients.
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
    [Mail.d.ts:62](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L62)

::: {.tsd-comment .tsd-typography}
::: {.lead}
whether to treat the body string and plain text or HTML. When set to
`true`, the `body` property should be set to full valid HTML.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#issent .tsd-anchor}

### isSent

::: {.tsd-signature .tsd-kind-icon}
isSent[:]{.tsd-signature-symbol} [boolean]{.tsd-signature-type}
:::

-   Defined in
    [Mail.d.ts:72](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L72)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Indicates if the message object has already been sent.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#sendinbackground .tsd-anchor}

### sendInBackground

::: {.tsd-signature .tsd-kind-icon}
sendInBackground[:]{.tsd-signature-symbol}
[boolean]{.tsd-signature-type}
:::

-   Defined in
    [Mail.d.ts:67](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L67)

::: {.tsd-comment .tsd-typography}
::: {.lead}
If `true`, the mail will be sent in the background using a web service
rather than via Mail.app - but will come from
`drafts5@drafts5.agiletortoise.com`. Defaults to `false`.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#status .tsd-anchor}

### status

::: {.tsd-signature .tsd-kind-icon}
status[:]{.tsd-signature-symbol}
[mailStatus](../globals.html#mailstatus){.tsd-signature-type}
:::

-   Defined in
    [Mail.d.ts:85](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L85)

::: {.tsd-comment .tsd-typography}
::: {.lead}
One of the following values:

-   created: Initial value before `send()` has been called.
-   sent: The message was sent successfully.
-   savedAsDraft: On iOS, the user exited the Mail.app window saving as
    draft, but not sending.
-   mailUnavailable: On iOS, Mail.app services were not available.
-   userCancelled: The user cancelled the Mail.app window without
    sending.
-   invalid: Mail object is invalid. Common cause if of this is
    sendInBackground being true, but no recipient configured.
-   serviceError: Background mail service returned an error.
-   unknownError: An unknown error occurred.
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
    [Mail.d.ts:52](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L52)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Subject line
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#torecipients .tsd-anchor}

### toRecipients

::: {.tsd-signature .tsd-kind-icon}
toRecipients[:]{.tsd-signature-symbol}
[string]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}
:::

-   Defined in
    [Mail.d.ts:37](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L37)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of email addresses to use as `To:` recipients.
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
        [Mail.d.ts:90](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L90)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Send the mail message. This will open the `Mail.app` sending window.
    Returns `true` if the message was sent successfully or `false` if
    not - if, for example, the user cancelled the mail window.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Mail](mail.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Mail.d.ts:95](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Mail.d.ts#L95)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create `Mail` object
    :::
    :::

    #### Returns [Mail](mail.html){.tsd-signature-type} {#returns-mail-1 .tsd-returns-title}
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
-   [Mail](mail.html){.tsd-kind-icon}
    -   [constructor](mail.html#constructor){.tsd-kind-icon}
    -   [bccRecipients](mail.html#bccrecipients){.tsd-kind-icon}
    -   [body](mail.html#body){.tsd-kind-icon}
    -   [ccRecipients](mail.html#ccrecipients){.tsd-kind-icon}
    -   [isBodyHTML](mail.html#isbodyhtml){.tsd-kind-icon}
    -   [isSent](mail.html#issent){.tsd-kind-icon}
    -   [sendInBackground](mail.html#sendinbackground){.tsd-kind-icon}
    -   [status](mail.html#status){.tsd-kind-icon}
    -   [subject](mail.html#subject){.tsd-kind-icon}
    -   [toRecipients](mail.html#torecipients){.tsd-kind-icon}
    -   [send](mail.html#send){.tsd-kind-icon}
    -   [create](mail.html#create){.tsd-kind-icon}

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
