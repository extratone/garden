---
{"dg-publish":true,"permalink":"/email/re-x-callback-url-support-in-tusker/","dgHomeLink":true,"dgPassFrontmatter":false}
---

Updated `10112022-110052`

- [Spark Thread](https://app.sparkmailapp.com/web-share/TLxvNNFPztMiSCEHi7URSOLg2SnkQLwe2px7fGI6)
- [Spark Local](readdle-spark://bl=QTphc3BoYWx0YXBvc3RsZUBpY2xvdWQuY29tO0lEOjczRDdCMzQ5LUMxQkUtNEE3%0D%0AQi04OEYwLTM4MTRDMkFCM0NBOEBzaGFkb3dmYWN0cy5uZXQ7MTI0MDYxOTgwMA%3D%3D)
- [WTF](https://davidblue.wtf/drafts/575B0F29-5C7E-4214-AF56-B41D1C3F36FD.html)
- [WTF Shortlink](https://davidblue.wtf/tuskerx) - `https://davidblue.wtf/tuskerx`
- [Local](shareddocuments:///private/var/mobile/Library/Mobile%20Documents/com~apple~CloudDocs/Written/575B0F29-5C7E-4214-AF56-B41D1C3F36FD.md)
- [Re: X-Callback-URL Support in Tusker](https://chaff.writeas.com/re-x-callback-url-support-in-tusker)
- [Things](things:///show?id=3creemTz4FKmzLfnsCtFtZ)

---

## Social

<script async="" src="https://telegram.org/js/telegram-widget.js?1" data-telegram-post="extratone/12963" data-width="100%"></script>

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">what an eloquent response!<br><br>though the news is quite unfortunate for me at least. <a href="https://t.co/1vfpNf7Css">https://t.co/1vfpNf7Css</a></p>&mdash; 𝗗 𝗔 𝗩 𝗢 𝗗 (@NeoYokel) <a href="https://twitter.com/NeoYokel/status/1579864906639478784?ref_src=twsrc%5Etfw">October 11, 2022</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

- [Telegram](https://t.me/extratone/12963)
- [Twitter](https://twitter.com/NeoYokel/status/1579864906639478784)

what an eloquent response!

though the news is quite unfortunate for me at least. https://davidblue.wtf/tuskerx

---

From: Shadowfacts <me@shadowfacts.net>
To: David Blue <davidblue@extratone.com>
Date: Oct 11, 2022
Subject: Re: X-Callback-URL Support in Tusker

Hi,

Thanks for reaching out. I can only speak to my reasons—but I suspect they’re similar across the industry.

XCB support was a significant extra maintenance burden that was both fragile and largely unused (I don’t have the analytics to be certain, but I strongly suspect Tusker’s had literally zero usage because it had been broken for quite some time and no one reported it.).

Tusker’s XCB support predates parameterized shortcuts (indeed, that inability was the impetus for building it) and it has not kept up well over the past years of architectural changes to the app. Combined with the fact that the iOS automation/power-user scene has almost entirely moved to Shortcuts.app, the cost of maintaining a parallel and unused set of functionality isn’t worth it.

As I push toward an App Store release after over 4 years of development, I’m trying to make sure everything is in a good, long-term stable place—and the XCB implementation was not.

Tusker’s Shortcuts support is currently lacking, but I intend to add functionality comparable to what was previously possible with XCB URLs, so you won’t be without automation forever.

—Shadowfacts

> On Oct 10, 2022, at 2:41 PM, David Blue <davidblue@extratone.com> wrote:  
>
> Hello!  
> I realize it's honestly a bit incredulous that I'm choosing this of all Tusker topics to actually reach out to you about for the first time but...  
> I happened to catch this at the bottom of the release notes for today's Testflight build:  
> > X-Callback-URL support has been removed.  
> ...and dang... frankly, I was just very very saddened and upset with myself for having managed to miss its implementation in the first place!  
> This, however, is not a complaint email, nor even a suggestion email, actually. As someone who has only just recently found TREMENDOUS value in X-Callback-URLs and URL schemes in my own day to day computing life, this is actually a recurring experience of mine. I've more or less stopped reaching out to proprietary organizations about it, though. (I'm sure you can imagine why.)  
> I don't know anything about you except what I've seen in Tusker, and it is more than enough to compel me to ask you, specifically...  
> Is there some overarching reason why folks have now begun actively removing their X-Callback-URL support instead of (frankly) just forgetting about it?  
> Obviously, I consider any time of yours spent answering this to be purely a favor, so it does not come with anything like obligation or time-sensitivity.  
> I am kinda starting to worry about the issue tho lol.  
> Thanks for your time!  
> 𝗗𝗮𝘃𝗶𝗱 𝗕𝗹𝘂𝗲  