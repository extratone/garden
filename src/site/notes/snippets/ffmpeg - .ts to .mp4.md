---
{"dg-publish":true,"permalink":"/snippets/ffmpeg-ts-to-mp4/","dgHomeLink":true,"dgPassFrontmatter":false}
---

ffmpeg - .ts to .mp4
ffmpeg -i input.ts -c:v libx264 -c:a aac output.mp4

ffmpeg -i unclegoogle.ts -c:v libx264 -c:a aac unclegoogle.mp4

Tags:
  conversion, media, snippets