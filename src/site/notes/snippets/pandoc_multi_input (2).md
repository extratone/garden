---
{"dg-publish":true,"permalink":"/snippets/pandoc-multi-input-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

pandoc_multi_input (2)

---
created: 2021-05-08T21:41:57Z
folder: Gist
gist: https://gist.github.com/997d55f8d23f2bd40932bbe484b92a5f
language: Markdown
modified: 2022-03-23T04:43:31Z
notes: |
    Combine multiple input files when using Pandoc
    Author: extratone (https://gist.github.com/997d55f8d23f2bd40932bbe484b92a5f)
title: pandoc_multi_input.md
---

> If multiple input files are given, pandoc will concatenate them all (with blank lines between them) before parsing. -- from Pandoc website

Pandoc command:
`pandoc -s input1.md input2.md input3.md -o output.html`

pandoc -s *.txt -o .txt
pandoc -s *.html -o .md