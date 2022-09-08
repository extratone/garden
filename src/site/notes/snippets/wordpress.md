---
{"dg-publish":true,"permalink":"/snippets/wordpress/","dgHomeLink":true,"dgPassFrontmatter":false}
---

wordpress

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
-   [WordPress](wordpress.html)

Class WordPress
===============
:::
:::

::: {.container .container-main}
::: {.row}
::: {.col-8 .col-content}
::: {.section .tsd-panel .tsd-comment}
::: {.tsd-comment .tsd-typography}
::: {.lead}
[](#wordpress){#wordpress}

WordPress
=========
:::

Script integration with WordPress sites via the [WordPress XML-RPC
API](https://codex.wordpress.org/XML-RPC_WordPress_API). Currently this
object has one runMethod function which can be used to call any method
available in the XML-RPC interface.

The WordPress API offers access to a wide variety of functions,
including posting, but also retrieving information about categories and
tags, or reading posts contents.

Drafts `WordPress` object simplifies working with the XML-RPC interface
by accepting input parameters as Javascript objects and converting them
to the require XML to make requests of the WordPress site. Similarly, it
converts to XML returned by WordPress to Javascript objects. Otherwise
it is an exact passthrough, so the [WordPress API
reference](https://codex.wordpress.org/XML-RPC_WordPress_API) should be
used to determine method names (e.g. `wp.newPost`, `wp.getTaxonomies`)
available, the appropriate parameters to send.

The WordPress XML-RPC API authenticates via username and password, so it
is highly recommended you interact only over HTTPS secure connections,
and use `Credential` objects to store host/username/password values,
rather than hard-coding them in actions.

[](#example){#example}

### Example

    // setup values to use in post
    let title = "Title of Post"
    let body = "Body of Post"

    // create credentials for site
    let cred = Credential.createWithHostUsernamePassword("WordPress", "WordPress  * credentials. Include full URL (with http://) of the home page of your WordPress  * site in the host field.");
    cred.authorize();

    // create WordPress object and make request
    let wp = WordPress.create(cred.getValue("host"), 1, "", "");
    let method = "wp.newPost"
    let params = [
        1, // blog_id, in most cases just use 1
        cred.getValue("username"),
        cred.getValue("password"),
        {
            "post_title": title,
            "post_content": body,
            "post_status": "draft",
            "terms_names" : { // assign categories and tags
                "category" : ["Cat1", "BAD"],
                "post_tag" : ["Test1", "NOT-TAG"]
            }
        }
    ];

    let response = wp.runMethod(method, params);
    if (response.success) {
        let params = response.params;
        console.log("Create WordPress post id: " + params[0]);
    }
    else {
        console.log("HTTP Status: " + response.statusCode);
        console.log("Fault: " + response.error);
        context.fail();
    }
:::
:::

::: {.section .tsd-panel .tsd-hierarchy}
### Hierarchy

-   [WordPress]{.target}
:::

::: {.section .tsd-panel-group .tsd-index-group}
Index
-----

::: {.section .tsd-panel .tsd-index-panel}
::: {.tsd-index-content}
::: {.section .tsd-index-section}
### Constructors

-   [constructor](wordpress.html#constructor){.tsd-kind-icon}
:::

::: {.section .tsd-index-section}
### Methods

-   [getCategories](wordpress.html#getcategories){.tsd-kind-icon}
-   [getPost](wordpress.html#getpost){.tsd-kind-icon}
-   [getPostStatusList](wordpress.html#getpoststatuslist){.tsd-kind-icon}
-   [getPosts](wordpress.html#getposts){.tsd-kind-icon}
-   [getTags](wordpress.html#gettags){.tsd-kind-icon}
-   [getTaxonomies](wordpress.html#gettaxonomies){.tsd-kind-icon}
-   [getTaxonomy](wordpress.html#gettaxonomy){.tsd-kind-icon}
-   [getTerms](wordpress.html#getterms){.tsd-kind-icon}
-   [newPost](wordpress.html#newpost){.tsd-kind-icon}
-   [runMethod](wordpress.html#runmethod){.tsd-kind-icon}
-   [create](wordpress.html#create){.tsd-kind-icon}
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

-   new WordPress[(]{.tsd-signature-symbol}siteURL[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, blogId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, username[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, password[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[WordPress](wordpress.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:84](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L84)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance
    :::
    :::

    #### Parameters {#parameters .tsd-parameters-title}

    -   ##### siteURL: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        ::: {.lead}
        This should be the full URL to the home page of the WordPress
        site. e.g. `https://mysite.com` or `https://mysite.com/blog/`.
        :::
        :::

    -   ##### blogId: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        ::: {.lead}
        For most WordPress installations, use `1`.
        :::
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} username: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        ::: {.lead}
        Username to login to the WordPress site. Optional if only using
        runMethod, as credentials will be required directly in
        parameters for those calls.
        :::
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} password: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        ::: {.lead}
        Password to login to the WordPress site. Optional if only using
        runMethod, as credentials will be required directly in
        parameters for those calls.
        :::
        :::

    #### Returns [WordPress](wordpress.html){.tsd-signature-type} {#returns-wordpress .tsd-returns-title}
:::
:::

::: {.section .tsd-panel-group .tsd-member-group}
Methods
-------

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getcategories .tsd-anchor}

### getCategories

-   getCategories[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:62](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L62)

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getpost .tsd-anchor}

### getPost

-   getPost[(]{.tsd-signature-symbol}postId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:55](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L55)

    #### Parameters {#parameters-1 .tsd-parameters-title}

    -   ##### postId: [string]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined-1 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getpoststatuslist .tsd-anchor}

### getPostStatusList

-   getPostStatusList[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:58](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L58)

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined-2 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getposts .tsd-anchor}

### getPosts

-   getPosts[(]{.tsd-signature-symbol}filter[?:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:57](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L57)

    #### Parameters {#parameters-2 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} filter: [any]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined-3 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettags .tsd-anchor}

### getTags

-   getTags[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:63](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L63)

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined-4 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettaxonomies .tsd-anchor}

### getTaxonomies

-   getTaxonomies[(]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:60](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L60)

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined-5 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#gettaxonomy .tsd-anchor}

### getTaxonomy

-   getTaxonomy[(]{.tsd-signature-symbol}taxonomy[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:59](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L59)

    #### Parameters {#parameters-3 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} taxonomy: [string]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined-6 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#getterms .tsd-anchor}

### getTerms

-   getTerms[(]{.tsd-signature-symbol}taxonomy[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, filter[?:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[
    \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:61](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L61)

    #### Parameters {#parameters-4 .tsd-parameters-title}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} taxonomy: [string]{.tsd-signature-type}

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} filter: [any]{.tsd-signature-type}

    #### Returns [object]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-object-undefined-7 .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#newpost .tsd-anchor}

### newPost

-   newPost[(]{.tsd-signature-symbol}content[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[ \|
    ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:56](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L56)

    #### Parameters {#parameters-5 .tsd-parameters-title}

    -   ##### content: [string]{.tsd-signature-type}

    #### Returns [string]{.tsd-signature-type}[ \| ]{.tsd-signature-symbol}[undefined]{.tsd-signature-type} {#returns-string-undefined .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class}
[]{#runmethod .tsd-anchor}

### runMethod

-   runMethod[(]{.tsd-signature-symbol}methodName[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, parameters[:
    ]{.tsd-signature-symbol}[any]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[XMLRPCResponse](xmlrpcresponse.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:70](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L70)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Run an XML-RPC API method on a WordPress site. Any method name
    supported by the [WordPress XML-RPC
    API](https://codex.wordpress.org/XML-RPC_WordPress_API) can be used,
    as long as the authentication information provided has appropriate
    permissions on the site.
    :::
    :::

    #### Parameters {#parameters-6 .tsd-parameters-title}

    -   ##### methodName: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        The method name as documented in the WordPress XML-RPC API, for
        example `wp.newPost` to create a new post.
        :::

    -   ##### parameters: [any]{.tsd-signature-type}[\[\]]{.tsd-signature-symbol}

        ::: {.tsd-comment .tsd-typography}
        Parameters should be a Javascript array of parameters for the
        method being used. These vary depending on the method and should
        follow the documentation provided by WordPress.
        :::

    #### Returns [XMLRPCResponse](xmlrpcresponse.html){.tsd-signature-type} {#returns-xmlrpcresponse .tsd-returns-title}
:::

::: {.section .tsd-panel .tsd-member .tsd-kind-method .tsd-parent-kind-class .tsd-is-static}
[]{#create .tsd-anchor}

### [Static]{.tsd-flag .ts-flagStatic} create

-   create[(]{.tsd-signature-symbol}siteURL[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, blogId[:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, username[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}, password[?:
    ]{.tsd-signature-symbol}[string]{.tsd-signature-type}[)]{.tsd-signature-symbol}[:
    ]{.tsd-signature-symbol}[WordPress](wordpress.html){.tsd-signature-type}

```{=html}
<!-- -->
```
-   -   Defined in
        [WordPress.d.ts:79](https://github.com/agiletortoise/drafts-script-reference/blob/bb281e8/src/WordPress.d.ts#L79)

    ::: {.tsd-comment .tsd-typography}
    ::: {.lead}
    Create new instance
    :::
    :::

    #### Parameters {#parameters-7 .tsd-parameters-title}

    -   ##### siteURL: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        This should be the full URL to the home page of the WordPress
        site. e.g. `https://mysite.com` or `https://mysite.com/blog/`.
        :::

    -   ##### blogId: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        For most WordPress installations, use `1`.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} username: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Username to login to the WordPress site. Optional if only using
        runMethod, as credentials will be required directly in
        parameters for those calls.
        :::

    -   ##### [Optional]{.tsd-flag .ts-flagOptional} password: [string]{.tsd-signature-type}

        ::: {.tsd-comment .tsd-typography}
        Password to login to the WordPress site. Optional if only using
        runMethod, as credentials will be required directly in
        parameters for those calls.
        :::

    #### Returns [WordPress](wordpress.html){.tsd-signature-type} {#returns-wordpress-1 .tsd-returns-title}
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
-   [WordPress](wordpress.html){.tsd-kind-icon}
    -   [constructor](wordpress.html#constructor){.tsd-kind-icon}
    -   [getCategories](wordpress.html#getcategories){.tsd-kind-icon}
    -   [getPost](wordpress.html#getpost){.tsd-kind-icon}
    -   [getPostStatusList](wordpress.html#getpoststatuslist){.tsd-kind-icon}
    -   [getPosts](wordpress.html#getposts){.tsd-kind-icon}
    -   [getTags](wordpress.html#gettags){.tsd-kind-icon}
    -   [getTaxonomies](wordpress.html#gettaxonomies){.tsd-kind-icon}
    -   [getTaxonomy](wordpress.html#gettaxonomy){.tsd-kind-icon}
    -   [getTerms](wordpress.html#getterms){.tsd-kind-icon}
    -   [newPost](wordpress.html#newpost){.tsd-kind-icon}
    -   [runMethod](wordpress.html#runmethod){.tsd-kind-icon}
    -   [create](wordpress.html#create){.tsd-kind-icon}

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
