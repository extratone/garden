---
{"dg-publish":true,"permalink":"/drafts/ded-78-e44-fcea-4-ea-1-8-cd-6-5-e635-f05-cfb-1-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

Updated `09072022-151246`

- [Lost text, version issue?](https://forums.getdrafts.com/t/lost-text-version-issue/13270)
- [WTF](https://davidblue.wtf/drafts/DED78E44-FCEA-4EA1-8CD6-5E635F05CFB1.html)


## Social

- [Telegram](https://t.me/draftsapp/279)

this exchange is quite informative, actually, and also highlights one of the big reasons why I have so much loyalty to this gosh darned application. https://forums.getdrafts.com/t/lost-text-version-issue/13270
---

lens | 2022-09-04 22:26:20 UTC | #1

Recently I saw text evaporate while I watched, when switching from one device to another.  I use Drafts daily, usually have the same draft open on several devices and add to it using whichever is more convenient, phone if that's all I have, mac or ipad as available.

The first time I noticed this, I flailed around trying to recover the text with undo, looking into backups, etc., without success.  After that I watched carefully every time I went to Drafts, and found that the problem occurred very occasionally and not in a way that I could predict.  So I stopped switching devices without running a manual backup, which is of course not a smooth workflow.

Context:
iPhone SE, MXVL2LL/A, ios 14.8 (15.6.1 latest available), drafts v27.0.11 (v32.2 available)
iPad 6th gen, MR752LL/A, ios 14.4.2, (15.6.1 available) drafts v28.0.40 (v32.2 available)
Macbook Pro M1, macos 12.3.1 Monterey (12.5.1 available), drafts v31.1.1 (41) (v32.2 available)

Yes, it's a hodge-podge of versions and I'll update things.  And I noticed that I hadn't subscribed in spite of good intentions, so I just did that.  Meanwhile, I have lost some text and would certainly appreciate help making the best of things.  Drafts has been so good for so long that I got complacent.

So, questions:
(1) I assume losing text is an artifact of some failure on my part, but what is it?  Do all versions of Drafts have to be the same?

(2) Is there some way to prevent losing text in this situation without going to Settings and running a backup manually?  I typically live in a draft for a few hours or days until I create another.  "New Draft Creation" is set to "Never".

(2) Is there any way to find out whether I have lost other text without noticing?  I am concerned because I frequently don't study the screen while opening up a device, and often have my eyes elsewhere while my hands are getting the device going.  And I don't usually review text immediately.  I count on Drafts to supplement my memory!

(3) Is there any way to recover lost text?  I found Community exchanges with BurnNorton dated Jan 19 and hobbyist in Nov 19 that suggest looking in prior versions.  But I'm concerned because one of the triggers for version creation is when loading a different draft, and my issue occurs when editing the same draft through the day, on several devices.

Thanks for your help!
lens

-------------------------

agiletortoise | 2022-09-04 23:37:40 UTC | #2

Drafts sync is a "last edit wins" sync strategy. Sync is usually very fast, but if you actively edit the same draft on multiple devices, it's not too hard to create a situation where you edit on a device before a change from another device has a chance to arrive.

Drafts is also generally optimized around not interrupting you. So, if a conflict occurs, the app saves the conflicted version in the version history. You should never lose anything in these situations, just check the [version history](https://docs.getdrafts.com/docs/drafts/versionhistory) of the draft. You should never need to resort to backups or anything.

There are valid arguments that Drafts should interrupt you and let you know about the conflict. That strategy is pretty intrusive, and hasn't been requested often, so I've never pursued it.

As far as versions of Drafts? This should not specifically have led to anything you are describing, but yes, you should absolutely keep the app up to date and running close to the same version on all devices. Consider just enabling automatic updates in the App Store. It's a big deal for bug fixes, and compatibility.

-------------------------

lens | 2022-09-05 02:44:16 UTC | #3

Thanks for the insight. So if I see the last change on one device appear on another, it should be safe to continue?  Of course changes can be more complicated than additions to the end of the text. 

It seems that the cell phone and wifi ipad instances of Drafts would be vulnerable to sync issues when going in and out of wifi range. I do that reasonably often, toting the ipad along in the car with its cellular data connection turned off to save data charges and battery. 

Regarding recovering text from the per-draft version history, are those entries time stamped with fine granularity?  I wonder about building a tool to look for cross device sync issues and hand repair them. 

Thanks again
lens

-------------------------