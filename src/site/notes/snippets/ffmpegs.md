---
{"dg-publish":true,"permalink":"/snippets/ffmpegs/","dgHomeLink":true,"dgPassFrontmatter":false}
---

ffmpegs

---
created: 2021-06-29T16:25:44Z
folder: Gist
gist: https://gist.github.com/9d00edb567ec982408c5bb5d523beaa5
language: Markdown
modified: 2021-06-29T16:25:45Z
notes: |
    My personal collection of ffmpeg one-liners.
    Author: extratone (https://gist.github.com/9d00edb567ec982408c5bb5d523beaa5)
title: ffmpegs.md
---

1. Converting .ts files to .mp4 files with ffmpeg.
`ffmpeg -i xperia.ts -c:v libx264 -c:a aac xperia.mp4`

2. Converting .mov to mp4.
`ffmpeg -i decision.mov -vcodec h264 -acodec mp2 decision.mp4`