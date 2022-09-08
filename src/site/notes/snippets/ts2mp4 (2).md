---
{"dg-publish":true,"permalink":"/snippets/ts2mp4-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

ts2mp4 (2)

---
created: 2021-06-29T07:39:31Z
folder: Gist
gist: https://gist.github.com/e497bbd8ac132abc370f10c28e4ead81
language: Markdown
modified: 2021-06-29T07:39:31Z
notes: |
    Converting .ts files to .mp4 files with ffmpeg.
    Author: extratone (https://gist.github.com/e497bbd8ac132abc370f10c28e4ead81)
title: ts2mp4.md
---

```
ffmpeg -i xperia.ts -c:v libx264 -c:a aac xperia.mp4
```