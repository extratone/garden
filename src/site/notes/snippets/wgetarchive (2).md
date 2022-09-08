---
{"dg-publish":true,"permalink":"/snippets/wgetarchive-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

wgetarchive (2)

---
created: 2021-03-28T19:18:43Z
folder: Gist
gist: https://gist.github.com/fe1cd3ea325c48d50d82ae24b9ba748e
language: Markdown
modified: 2021-06-07T07:02:19Z
notes: |
    A single-line command for wget that *actually* builds an archive of a given domain. 
    Author: extratone (https://gist.github.com/fe1cd3ea325c48d50d82ae24b9ba748e)
title: wgetarchive.md
---

## Customized (For my use.)

```
wget -e robots=off -R mpg,mpeg,mp4,mov,wav,tgz,zip,flv --recursive --page-requisites --adjust-extension --span-hosts --convert-links --restrict-file-names=windows --domains bilge.world --no-parent bilge.world
```

```
wget --recursive --page-requisites --adjust-extension --span-hosts --convert-links --restrict-file-names=windows --domains extratone.com --no-parent extratone.com
```

* [**Original source!**](https://gist.github.com/mikecrittenden/fe02c59fed1aeebd0a9697cf7e9f5c0c)