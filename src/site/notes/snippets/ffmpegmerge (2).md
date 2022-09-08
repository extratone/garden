---
{"dg-publish":true,"permalink":"/snippets/ffmpegmerge-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

ffmpegmerge (2)

---
created: 2021-09-20T20:56:33Z
folder: Gist
gist: https://gist.github.com/e8c9839797d6766383580480b4bb5961
language: Markdown
modified: 2021-09-20T21:01:31Z
notes: |
    How to merge ("Concatenate") two .mp4 files with ffmpeg... Sorry, I just cannot for the life of me figure out another way to not forget this when I need it.
    Author: extratone (https://gist.github.com/e8c9839797d6766383580480b4bb5961)
title: ffmpegmerge.md
---

**Create a .txt file in the following format in the same directory as the files to be merged.**

```txt
file '/downloads/152.mp4'
file '/downloads/151.mp4'
```
`ffmpeg -f concat -i [saidfile].txt -c copy output.mp4`

***
# Convert .mov file to .mp4 in a single command.
`ffmpeg -i obit.mov -vcodec h264 -acodec mp2 obit.mp4`