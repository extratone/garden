---
{"dg-publish":true,"permalink":"/snippets/periscopepreservation-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

periscopepreservation (2)

---
created: 2021-03-24T13:39:36Z
folder: Gist
gist: https://gist.github.com/614effdd51bac74793ef627a1174e972
language: Markdown
modified: 2021-03-25T13:35:22Z
notes: |
    An ongoing document for (former) Periscope users detailing all available means of preserving/scraping data and media from psp.tv.
    Author: extratone (https://gist.github.com/614effdd51bac74793ef627a1174e972)
title: periscopepreservation.md
---

# Periscope Preservation
## An ongoing document for (former) Periscope users detailing all available means of preserving/scraping data and media from psp.tv.

The [official announcement of Periscope's demise](https://periscope.medium.com/farewell-periscope-164db2742b7c) was posted on their Medium blog on December 15th, 2020.

It states:
> Broadcasts that were shared to Twitter will live on as replays, and all broadcasters will be able to download an archive of their Periscope broadcasts and data before the app is removed in March 2021.

Thanks to [a brief series of Tweets](https://twitter.com/twittersupport/status/1367173142188335114) from @TwitterSupport, we know **the app is going to be removed from the app store on March 31st**. (Which is in 8 days, atm.)

_However_, the hyperlink referenced for users to find "more info… about what will happen to your Super Hearts and broadcasts, how you can go live on Twitter going forward, and more" (https://help.twitter.com/using-twitter/periscope-faq) is **currently broken** as of Mar 24, 2021 at 08:20 (CST.) I have posted replies on both [Medium](https://extratone.medium.com/periscope-twitter-public-policy-5305341a9043) and [Twitter](https://twitter.com/NeoYokel/status/1374680479874568194) pinging the relevant accounts I could find.

Given the above pullquote from the blog post, this means Twitter/Periscope has 8 days to enable users to download "an archive of their Periscope broadcasts and data," but…

## The method for downloading "broadcasts and data" as documented by Twitter/Periscope does not currently work
* [Youtube-dl](http://ytdl-org.github.io/youtube-dl/) supports downloading Periscope broadcasts and is by far the best method I have discovered. (It even saves them as a .mp4 file with 0 configuration, at the moment.)
* [Scopedown](https://downloadperiscopevideos.com) is another, tried-and-true method of scraping full Periscope broadcasts in their native format, but will eventually obstruct you with a paywall.
* The page all current Periscope documentation eventually points you to (https://www.pscp.tv/account/your-data) in order to "download your data" **currently results only in a virtually useless .JSON file** (it only includes broadcast IDs and some bewildering timestamp-related data.)

***
Any/all thoughts/feedback/corrections/updates would be deeply appreciated here on Github, [by email](mailto:davidblue@extratone.com), [Twitter](https://twitter.com/NeoYokel), or [any other social platform](https://www.notion.so/rotund/Social-Directory-aea1bee51a64461b91bf4de241a4a16d).