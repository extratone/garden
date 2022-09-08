---
{"dg-publish":true,"permalink":"/snippets/credential/","dgHomeLink":true,"dgPassFrontmatter":false}
---

credential

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
-   [Credential](credential.html)

Class Credential
================
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#credential){#credential}

Credential
==========
:::

Credential objects can be used in actions which require the user to
provide a username, password and optionally a host name, to connect to a
service. By using credentials objects, actions can be written to connect
to arbitrary web services without hard coding credentials into the
action.

When an authorize() call is made on a credential object for the first
time, the user is prompted to enter their credentials, then Drafts
stores those for later use. When the action is used again, there will be
no prompt required and the stored credentials will be used.

Credentials objects have unique identifiers, and a single set of user
credentials can be used across actions by using the same identifier.

The user can delete those credentials at any time by visiting Settings
\> Credentials and tapping the \"Forget\" button on a service.

[](#example){#example}

### Example

    var credential = Credential.create("My Service", "Description of the service to  * appear in user prompt.");

    credential.addTextField("username", "Username");
    credential.addPasswordField("password", "Password");

    credential.authorize();

    var http = HTTP.create();
    var response = http.request({
      "url": "http://myurl.com/api",
      "username": credential.getValue("username"),
      "password": credential.getValue("password"),
      "method": "POST",
      "data": {
        "key":"value"
      },
      "headers": {
        "HeaderName": "HeaderValue"
      }
    });
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [Credential]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](credential.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [addPasswordField](credential.html#addpasswordfield){.tsd-kind-icon}
-   [addTextField](credential.html#addtextfield){.tsd-kind-icon}
-   [addURLField](credential.html#addurlfield){.tsd-kind-icon}
-   [authorize](credential.html#authorize){.tsd-kind-icon}
-   [forget](credential.html#forget){.tsd-kind-icon}
-   [getValue](credential.html#getvalue){.tsd-kind-icon}
-   [create](credential.html#create){.tsd-kind-icon}
-   [createWithHostUsernamePassword](credential.html#createwithhostusernamepassword){.tsd-kind-icon}
-   [createWithUsernamePassword](credential.html#createwithusernamepassword){.tsd-kind-icon}
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

-   new Credential[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type},
    description[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Credential](credential.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:64](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L64)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance.
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        ::: {.lead}
        Unique identifier for the credentials
        :::
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} description: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        ::: {.lead}
        Optional description
        :::
        :::

    #### Returns [Credential](credential.html){.tsd-signature-type} {#returns-credential .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addpasswordfield .tsd-anchor}

### addPasswordField

-   addPasswordField[(]{.tsd-signature-symbol}key[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:95](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L95)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a secure entry text field for data entry.
    :::
    :::

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### key: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        used to retrieve the value
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        label is displayed to the user
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addtextfield .tsd-anchor}

### addTextField

-   addTextField[(]{.tsd-signature-symbol}key[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:88](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L88)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a text field for data entry.
    :::
    :::

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### key: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        used to retrieve the value
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        label is displayed to the user
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#addurlfield .tsd-anchor}

### addURLField

-   addURLField[(]{.tsd-signature-symbol}key[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, label[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:102](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L102)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Add a text field for configured for URL data entry.
    :::
    :::

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### key: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        used to retrieve the value
        :::

    -   ##### label: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        label is displayed to the user
        :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#authorize .tsd-anchor}

### authorize

-   authorize[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[boolean]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:76](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L76)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Call this function after configuring, but before using host,
    username or password properties of a credential. If the credential
    object has not be previous authorized, the user will be prompted to
    enter their credentials before continuing. If the user has
    previously been prompt, this method will load previously provided
    information.
    :::
    :::

    #### Returns [boolean]{.tsd-signature-type} {#returns-boolean .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#forget .tsd-anchor}

### forget

-   forget[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[void]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:107](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L107)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Deletes the credentials provided by the user. This is the same as
    the user visiting settings and tapping \"Forget\" for the
    credentials.
    :::
    :::

    #### Returns [void]{.tsd-signature-type} {#returns-void-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getvalue .tsd-anchor}

### getValue

-   getValue[(]{.tsd-signature-symbol}key[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:81](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L81)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Get the value the user stored for the key, as defined in a call to
    add the field.
    :::
    :::

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### key: [string]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type} {#returns-string .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type},
    description[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Credential](credential.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:44](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L44)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create a credential object with the specified identifier and
    description. Identifiers should be unique, such that any two calls
    from different actions with the same identifier will return the same
    credentials
    :::
    :::

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Unique identifier for the credentials
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} description: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional description
        :::

    #### Returns [Credential](credential.html){.tsd-signature-type} {#returns-credential-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#createwithhostusernamepassword .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} createWithHostUsernamePassword

-   createWithHostUsernamePassword[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, description[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Credential](credential.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:61](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L61)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create credential already configured with host url, username and
    password fields.
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Unique identifier for the credentials
        :::

    -   ##### description: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional description
        :::

    #### Returns [Credential](credential.html){.tsd-signature-type} {#returns-credential-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#createwithusernamepassword .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} createWithUsernamePassword

-   createWithUsernamePassword[(]{.tsd-signature-symbol}identifier[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, description[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[Credential](credential.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [Credential.d.ts:51](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/Credential.d.ts#L51)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create credential already configured with username and password
    fields.
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### identifier: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Unique identifier for the credentials
        :::

    -   ##### description: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Optional description
        :::

    #### Returns [Credential](credential.html){.tsd-signature-type} {#returns-credential-3 .tsd-returns-title}
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
-   [Credential](credential.html){.tsd-kind-icon}
    -   [constructor](credential.html#constructor){.tsd-kind-icon}
    -   [addPasswordField](credential.html#addpasswordfield){.tsd-kind-icon}
    -   [addTextField](credential.html#addtextfield){.tsd-kind-icon}
    -   [addURLField](credential.html#addurlfield){.tsd-kind-icon}
    -   [authorize](credential.html#authorize){.tsd-kind-icon}
    -   [forget](credential.html#forget){.tsd-kind-icon}
    -   [getValue](credential.html#getvalue){.tsd-kind-icon}
    -   [create](credential.html#create){.tsd-kind-icon}
    -   [createWithHostUsernamePassword](credential.html#createwithhostusernamepassword){.tsd-kind-icon}
    -   [createWithUsernamePassword](credential.html#createwithusernamepassword){.tsd-kind-icon}

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
