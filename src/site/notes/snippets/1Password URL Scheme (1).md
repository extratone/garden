---
{"dg-publish":true,"permalink":"/snippets/1-password-url-scheme-1/","dgHomeLink":true,"dgPassFrontmatter":false}
---

1Password URL Scheme

Tags: x, macos, i
[1Password CLI Secret Reference Syntax | 1Password Developer Documentation](https://developer.1password.com/docs/cli/secrets-reference-syntax/)
---

Secret reference syntax
Learn how to create secret references that you can use to refer to secrets stored in 1Password.

With 1Password CLI, you can use secret references to inject secrets without editing the environment file or commands that you usually use to deploy your application. At runtime, secret references are replaced by the contents of the field that they reference in your 1Password account.

To reference a secret, use this syntax:

op://vault-name/item-name/[section-name/]field-name
If any of the names include an unsupported character, you can refer to it using its ID instead.

Secret reference examples​

A field inside a section​

To create a secret reference that refers to the PagerDuty email field, which is within the Admin section, use:

`op://Management/PagerDuty/Admin/email`

Management refers to the vault where the item is saved
PagerDuty refers to the item
Admin refers to the section where the field is a part of
email refers to the field where the secret you want to reference is located
PagerDuty 1Password item
A field without a section​

To create a secret reference for the Stripe publishable-key field, which is not part of a section, use:

`op://dev/Stripe/publishable-key`

dev refers to the vault where the item is saved
Stripe refers to the item
publishable-key refers to the field where the secret you want to reference is located
PagerDuty 1Password item
Syntax rules​

The following characters are allowed in secret references:

alphanumeric characters (a-z, A-Z, 0-9)
-, _, /, . and the whitespace character
Currently, secret references can't be used to reference Document items.

Learn more​

Load secrets into config files
Load secrets into the environment
Template syntax

Tags:
  i, snippets