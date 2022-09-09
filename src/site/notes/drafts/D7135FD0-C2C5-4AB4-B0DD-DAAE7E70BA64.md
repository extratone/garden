---
title: Drafts Autocompletes
tags: bookmarked, documentation, git, drafts
davodtime: 09082022-105520
local: shareddocuments:///private/var/mobile/Library/Mobile%20Documents/iCloud~md~obsidian/Documents/OBSHIDDIAN/drafts/D7135FD0-C2C5-4AB4-B0DD-DAAE7E70BA64.md
dg-publish: true
share: true
draft: drafts://open?uuid=D7135FD0-C2C5-4AB4-B0DD-DAAE7E70BA64
---
Updated `08162022-123908`

- [GitHub Issue](https://github.com/extratone/drafts/issues/31)
- [Directory of install URLS in the repo](https://github.com/extratone/drafts/blob/main/autocomplete)
- [Tilde](https://tilde.town/~extratone/drafts/autocompletes/)
- [WTF](https://davidblue.wtf/drafts/D7135FD0-C2C5-4AB4-B0DD-DAAE7E70BA64.html)
- [WTF Shortlink](https://davidblue.wtf/autocompletes) - `https://davidblue.wtf/autocompletes`
- [Things](things:///show?id=KgfMefYzLGHkVy1KzsLq8X)

---

![Drafts Autocompletes](https://user-images.githubusercontent.com/43663476/159809109-ef35410c-d052-4ed4-9388-aa7895d1c434.png)

This is a collection of my personal “[Autocomplete Suggestions](https://docs.getdrafts.com/docs/editor/autocomplete)” (identical to what [TextExpander](https://apps.apple.com/us/app/textexpander-keyboard/id1075927186) calls “snippets”) for Drafts, and they *are* installable, if you’d like.

*Definitely read [Tim Nahumck’s work on this feature](https://nahumck.me/drafts-29-autocomplete/) if you’re curious about it.*

#### Install
The hyperlinks on the expansion triggers will take you a corresponding plain text file containing the installation URL (which is, of course, the entire contents of each, encoded in a string.) Copy the full text of the URL, paste it in your web browser, and tap/click “Go” (or your equivalent)/key `RETURN` or `ENTER`. Regardless of platform, you should receive a prompt asking if you’d like to open it in Drafts.

Here’s a wee [demo video](https://user-images.githubusercontent.com/43663476/159810974-fa1531df-c0a5-4f1b-82f8-3fe11e31f36d.MOV):

<video controls>
  <source src="https://user-images.githubusercontent.com/43663476/159810974-fa1531df-c0a5-4f1b-82f8-3fe11e31f36d.MOV">
</video>

--- 

- [**wtf**](https://raw.githubusercontent.com/extratone/drafts/main/snippets/wtf.txt)
```
https://davidblue.wtf/drafts/[[uuid|uuid]].html
```

- [**x**](https://raw.githubusercontent.com/extratone/drafts/main/snippets/x.txt)
```
[[[display_title|[display_title]]]([[draft_open_url|draft_open_url]])
```

- [**latlong**](https://raw.githubusercontent.com/extratone/drafts/main/snippets/latlong.txt)
```
`[[latitude]]-[[longitude]]-09082022-105520`
```

- [**img**](https://raw.githubusercontent.com/extratone/drafts/main/snippets/img.txt)
```
![]([[clipboard|clipboard]])
```

- [**code**](https://raw.githubusercontent.com/extratone/drafts/main/snippets/code.txt)
```
[[clipboard|clipboard]]
```

- [**snap**](https://raw.githubusercontent.com/extratone/drafts/main/snippets/snap.txt)
```
[[clipboard|clipboard]]
```

- [**video**](https://raw.githubusercontent.com/extratone/drafts/main/snippets/video.txt)
```
<video controls>
  <source src="[[clipboard|clipboard]]">
</video>
```

- [**audio**](https://raw.githubusercontent.com/extratone/drafts/main/snippets/audio.txt)
```
<audio controls>
  <source src=“[[clipboard|clipboard]]”>
</audio>
```

![action Autocomplete](https://i.snap.as/wfGYx2WU.png)

- [**action**](https://raw.githubusercontent.com/extratone/drafts/main/autocomplete/action.txt)
```
[[[clipboard|[clipboard]]](drafts://x-callback-url/runAction?text=TEXT&action=[[clipboard%5D%5D)
```