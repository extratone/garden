---
{"dg-publish":true,"permalink":"/snippets/message/","dgHomeLink":true,"dgPassFrontmatter":false}
---

message

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
-   [Message](message.html)

Class Message
=============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#message){#message}

Message
=======
:::

The Message object can be used to create and send mail iMessages,
similar to those created by a \"Message\" action step.

[](#examples){#examples}

### Examples

    var msg = Message.create();
    msg.toRecipients = ["joe@sample.com"];
    msg.subject = "My test message";
    msg.body = "Body text";

    var success = msg.send();
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Message]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](message.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Properties

-   [body](message.html#body){.tsd-kind-icon}
-   [isSent](message.html#issent){.tsd-kind-icon}
-   [status](message.html#status){.tsd-kind-icon}
-   [subject](message.html#subject){.tsd-kind-icon}
-   [toRecipients](message.html#torecipients){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [send](message.html#send){.tsd-kind-icon}
-   [create](message.html#create){.tsd-kind-icon}
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

-   new Message[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Message](message.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Message.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Message.d.ts#L57)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Returns [Message](message.html){.tsd-signature-type} {#returns-message .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Properties
----------

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#body .tsd-anchor}

### body

::: {.tsd-signature .tsd-kind-icon}
body[:]{.tsd-signature-symbol} [string]{.tsd-signature-type}
:::

-   Defined in
    [Message.d.ts:28](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Message.d.ts#L28)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Body text of the mail message.
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
    [Message.d.ts:32](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Message.d.ts#L32)

::: {.tsd-comment .tsd-typography}
::: {.lead}
true/false flag indicated if the message object has already been sent.
:::
:::
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-property .tsd-parent-kind-class}
[]{#status .tsd-anchor}

### status

::: {.tsd-signature .tsd-kind-icon}
status[:]{.tsd-signature-symbol} [\"created\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"sent\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"messagesUnavailable\"]{.tsd-signature-type}[
\| ]{.tsd-signature-symbol}[\"userCancelled\"]{.tsd-signature-type}[ \|
]{.tsd-signature-symbol}[\"unknownError\"]{.tsd-signature-type}
:::

-   Defined in
    [Message.d.ts:42](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Message.d.ts#L42)

::: {.tsd-comment .tsd-typography}
::: {.lead}
One of the following strings

-   created: Initial value before `send()` has been called.
-   sent: The message was sent successfully.
-   messagesUnavailable: On iOS, Mail.app services were not available.
-   userCancelled: The user cancelled the Mail.app window without
    sending.
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
    [Message.d.ts:24](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Message.d.ts#L24)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Subject line. Only used if subject is enabled in Messages settings on
the device.
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
    [Message.d.ts:20](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Message.d.ts#L20)

::: {.tsd-comment .tsd-typography}
::: {.lead}
Array of phone numbers and email addresses to use as `To:` recipients.
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
        [Message.d.ts:52](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Message.d.ts#L52)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Send the message. This will open the `Messages.app` sending window.
    Returns `true` if the message was sent successfully or `false` if
    not - if, for example, the user cancelled the message window.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Message](message.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Message.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Message.d.ts#L57)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Instantiate `Message` object
    :::
    :::

    #### Returns [Message](message.html){.tsd-signature-type} {#returns-message-1 .tsd-returns-title}
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
-   [Message](message.html){.tsd-kind-icon}
    -   [constructor](message.html#constructor){.tsd-kind-icon}
    -   [body](message.html#body){.tsd-kind-icon}
    -   [isSent](message.html#issent){.tsd-kind-icon}
    -   [status](message.html#status){.tsd-kind-icon}
    -   [subject](message.html#subject){.tsd-kind-icon}
    -   [toRecipients](message.html#torecipients){.tsd-kind-icon}
    -   [send](message.html#send){.tsd-kind-icon}
    -   [create](message.html#create){.tsd-kind-icon}

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
