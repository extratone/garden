---
title: Draft to Apple Note
tags: js, configuration, actions, curation, documentation, rich, meta, shortcuts, notes, drafts
davodtime: 09082022-105522
local: shareddocuments:///private/var/mobile/Library/Mobile%20Documents/iCloud~md~obsidian/Documents/OBSHIDDIAN/drafts/FE5F3B54-B9D6-48FF-BBFD-BB699E380C4F.md
dg-publish: true
share: true
draft: drafts://open?uuid=FE5F3B54-B9D6-48FF-BBFD-BB699E380C4F
---
Updated `08072022-120219`

- [**Drafts Directory**](https://directory.getdrafts.com/a/2Bi)
- [GitHub Issue](https://github.com/extratone/drafts/issues/81)
- [Repo File](https://github.com/extratone/drafts/blob/main/actions/DrafttoAppleNote.draftsAction)
- [WTF](https://davidblue.wtf/drafts/FE5F3B54-B9D6-48FF-BBFD-BB699E380C4F.html)
- [App Store Link](https://apps.apple.com/us/app/notes/id1110145109)
- [Using Apple Notes with Drafts - Integration Guides - Drafts Community](https://forums.getdrafts.com/t/using-apple-notes-with-drafts/899)

---

## Social

- [Thread Reply](https://forums.getdrafts.com/t/using-apple-notes-with-drafts/899/21)
- [Telegram](https://t.me/draftsapp/241)

<script async="" src="https://telegram.org/js/telegram-widget.js?1" data-telegram-post="draftsapp/241" data-width="100%"></script>

Well folks! 

I thought I would take the opportunity to formalize a very small victory regarding this integration...

In [the upcoming versions of iOS/iPadOS/macOS](https://www.matthewcassinelli.com/ios16-actions-shortcuts/), Apple Notes' Siri Shortcuts actions *will* be supporting Rich Text. As of Developer Beta 4, now, I found myself formally setting up this configuration, so I thought I'd share it.

![Draft to Apple Note Shortcut](https://user-images.githubusercontent.com/43663476/183301287-5fe0275f-3f4b-4fb9-b4d5-979f07bff620.png)

- [**Drafts Directory**](https://directory.getdrafts.com/a/2Bi) (The Drafts action.)
- [**iCloud Share Link**](https://www.icloud.com/shortcuts/1944ea6b1a7849e7aa39c1c07a4b4bd6) (Its corresponding shared Siri Shortcut)
- [GitHub Issue](https://github.com/extratone/drafts/issues/81)
- [Example Result](https://www.icloud.com/notes/053P3w2CeSRPryGQcjadduzVA#Draft_to_Apple_Note) (Shared Apple Note)

The reason there's so much tomfoolery going on with the shortcut and its [Replace Text](https://matthewcassinelli.com/actions/replace-text/) actions: the native [Make Rich Text from Markdown](https://matthewcassinelli.com/actions/make-rich-text-from-markdown/) action seems to be struggling with non-UTF-8 (?) characters. If you'd like surer footing on that explanation, I'd be more than happy to indulge, but I suspect its just a temporary oversight through the betas.

Speaking of which, especially since my user account has a checkmark on the Directory now (! <3,) I assume I should leave this action in unlisted status until these Siri Shortcuts changes come in the first *public* OS builds?

## Shortcut

- [**iCloud Share Link**](https://www.icloud.com/shortcuts/1944ea6b1a7849e7aa39c1c07a4b4bd6)
- [Shortcut Repository File](https://github.com/extratone/drafts/blob/main/shortcuts/DrafttoAppleNote.shortcut)

### Description

Designed to be called exclusively by a Drafts action found here: https://directory.getdrafts.com/a/2Bi

See this issue on my Drafts-specific GitHub repository for more information: https://github.com/extratone/drafts/issues/81

My contact information:

Email: davidblue@extratone.com
Contact card: bit.ly/whoisdavidblue
RoutineHub Profile: https://routinehub.co/user/blue
GitHub: https://github.com/extratone/i
Telegram: t.me/extratone
Twitter: twitter.com/NeoYokel
Reddit: reddit.com/u/asphaltapostle
Mastodon: mastodon.social/@DavidBlue
EVERYWHERE: bit.ly/dbrolodex

## Description

Runs a Siri Shortcut entitled "Draft to Apple Note" with the current draft's content passed as input in the following format:
```
[display_title]
[body]
```

## Directory Description

![Draft to Apple Note Shortcut](https://user-images.githubusercontent.com/43663476/183301287-5fe0275f-3f4b-4fb9-b4d5-979f07bff620.png)

*Please note: iOS/iPadOS Developer Betas 4 are required to run this action/shortcut pair.*

This action calls a Siri Shortcut entitled "[**Draft to Apple Note**](https://www.icloud.com/shortcuts/1944ea6b1a7849e7aa39c1c07a4b4bd6)," passing the current draft's contents in the following format:

```
[display_title]
[body]
```

<img src="https://user-images.githubusercontent.com/43663476/183300508-7c0812a9-9c22-4ad1-aeeb-c3533f4c0519.png" width="30%"></img>

---

## JS

```js
```

---

## Install

```
drafts://action?data=%7B%22uuid%22:%22ABA055F4-BDDA-4AE8-990E-E2DFE142C622%22,%22steps%22:%5B%7B%22platforms%22:3,%22data%22:%7B%22shortcutID%22:%22%22,%22waitForResponse%22:%22true%22,%22returnToDrafts%22:%22true%22,%22shortcutName%22:%22Draft%20to%20Apple%20Note%22,%22template%22:%22%5B%5Bdisplay_title%5D%5D%5Cn%5B%5Bbody%5D%5D%22,%22templateType%22:%22legacy%22%7D,%22type%22:%22runShortcut%22,%22isEnabled%22:true,%22uuid%22:%225B741902-B479-4286-B38F-4342EE65F22E%22%7D%5D,%22backingPlatforms%22:3,%22shortName%22:%22%22,%22shouldConfirm%22:false,%22disposition%22:0,%22keyCommand%22:%7B%22optionKey%22:true,%22input%22:%22A%22,%22controlKey%22:false,%22commandKey%22:false,%22type%22:%22action%22,%22discoverabilityTitle%22:%22Draft%20to%20Apple%20Note%22,%22shiftKey%22:false%7D,%22logLevel%22:2,%22groupDisposition%22:0,%22notificationType%22:2,%22tintColor%22:%22yellow%22,%22actionDescription%22:%22Runs%20a%20Siri%20Shortcut%20entitled%20%5C%22Draft%20to%20Apple%20Note%5C%22%20with%20the%20current%20draft's%20content%20passed%20as%20input%20in%20the%20following%20format:%5Cn%5Cn%60%60%60%5Cn%5Bdisplay_title%5D%5Cn%5Bbody%5D%5Cn%60%60%60%22,%22keyUseIcon%22:false,%22icon%22:%22memo%22,%22visibility%22:96,%22backingIsSeparator%22:false,%22groupUUID%22:%22DB5C51F1-9C68-4DE6-A310-33180D6E784D%22,%22assignTags%22:%5B%5D,%22name%22:%22Draft%20to%20Apple%20Note%22%7D
```