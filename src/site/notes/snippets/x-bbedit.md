---
{"dg-publish":true,"permalink":"/snippets/x-bbedit/","dgHomeLink":true,"dgPassFrontmatter":false}
---

x-bbedit

---
created: 2022-03-22T11:22:53Z
folder: Gist
gist: https://gist.github.com/fad566227f81d12c4468149ea293585b
language: Markdown
modified: 2022-03-22T11:22:53Z
notes: |
    Excerpt  from BBEdit's User Manual regarding its URL Scheme/x-callback-url support.
    Author: extratone (https://gist.github.com/fad566227f81d12c4468149ea293585b)
title: x-bbedit.md
---

BBEdit now supports using the ‘x-bbedit’ URL scheme for opening files, and optionally specifying destination line and column numbers. The syntax for this scheme is:

`x-bbedit://open?url=file:///path/to/some/file`

where ‘/path/to/some/file’ is the actual path to the file you want BBEdit to open. 

You can also specify a specific line to select when opening the file; for example: `x-bbedit://open?url=file:///path/to/some/file&line=5`

or if you also include add a column position, then BBEdit will place the insertion point before the indicated character on the previously-specified line:
`x-bbedit://open?url=file:///path/to/some/file&line=5&column=42`
Try clicking on this URL, and you’ll see that it opens one of your local files in BBEdit, even though you’re viewing it in a browser window:

`x-bbedit://open?url=file:///etc/hosts`

An ‘x-bbedit’ URL is guaranteed to launch BBEdit when opened from another application, unlike ‘file’ or ‘editor’ URLs, which are at the mercy of the OS to decide which application should open any given file.