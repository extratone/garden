---
{"dg-publish":true,"permalink":"/snippets/downloading-a-you-tube-channel-with-yt/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Downloading a YouTube channel with yt-dlp
Updated `08182022-075016`

- [Downloading a YouTube channel with yt-dlp](https://write.corbpie.com/downloading-a-youtube-channel-with-yt-dlp/)
- [Drafts](drafts://open?uuid=CAABBB06-186C-437D-BC30-65844BDBEC2B)
- [WTF](https://davidblue.wtf/drafts/CAABBB06-186C-437D-BC30-65844BDBEC2B.html)
- Simplenote Local
- Simplenote Publish
- Things

---

```
yt-dlp -f 'bv*[height>=720]+ba' --embed-thumbnail --embed-metadata --download-archive GetClearTouch.txt https://www.youtube.com/c/GetClearTouch/videos -o '%(channel)s/%(title)s.%(ext)s'
```

Tags:
  documentation, reference, scrape, simplenote, snippets, streaming, yt-dlp