---
{"dg-publish":true,"permalink":"/snippets/wget/","dgHomeLink":true,"dgPassFrontmatter":false}
---

wget

---
created: 2022-01-10T10:56:17Z
folder: Gist
gist: https://gist.github.com/2d7d8509d5d9abbc30c0d694c9dedc4c
language: Markdown
modified: 2022-01-10T10:56:17Z
notes: |
    Recursive wget ignoring robots
    Author: extratone (https://gist.github.com/2d7d8509d5d9abbc30c0d694c9dedc4c)
title: wget.md
---

    $ wget -e robots=off -r -np 'http://example.com/folder/'

* -e robots=off causes it to ignore robots.txt for that domain
* -r makes it recursive
* -np = no parents, so it doesn't follow links up to the parent folder