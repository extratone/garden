---
{"dg-publish":true,"permalink":"/snippets/url-scheme-binding-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

URLSchemeBinding-2

---
created: 2022-05-21T08:12:51Z
folder: Gist
gist: https://gist.github.com/28d31ac297461cf6c8c49d8d598bd31c
language: Markdown
modified: 2022-05-21T08:12:51Z
notes: |
    Usng lsregister -dump URLSchemeBinding.
    Author: extratone (https://gist.github.com/28d31ac297461cf6c8c49d8d598bd31c)
title: URLSchemeBinding.md
---

# URLScheme Binding
- [SnippetsLab](snippetslab://snippet/7B003932-54F1-428A-B26B-3617216D2A31/)
- [applications - What are all of the URI Schemes Available on macOS - Ask Different](https://apple.stackexchange.com/questions/397187/what-are-all-of-the-uri-schemes-available-on-macos)
- [URLSchemeBinding](drafts://open?uuid=A64BB28B-D251-4EB8-82BA-027F4A5BD1E9)
---

Use `lsregister`

The command can be found in `/System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister`. I suggest creating a symlink to one of the directories in your PATH for easy access.

You can copy and past the following command for simplicity:

`sudo ln -s /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister /usr/local/bin/lsregister`

Now, you can run `lsregister` from anywhere.

## Dump the URL Binding Table

`lsregister` has a number of database tables that contain various application registration details. The table that we're interested in is `URLSchemeBinding`

```
lsregister -dump URLSchemeBinding
```


This will give you the full list from `afp://` to `x-man-page://`.

To find the URL scheme used for the dictionary we can grep for it:

`lsregister -dump URLSchemeBinding | grep "dict*`

---
### Brief Example
```
dict:               35608 (0x8b18) (0x8b1a)
x-dictionary:       35604 (0x8b14) (0x8b16)
```




---
- vnc://----vnc URL (0x3040) (0x3042)
- applescript://--------AppleScript (0x33d4) (0x33d6)
- x-apple-helpbasic://----12164 (0x2f84) (0x2f86)
- ipps://----AirPrint (0x2fe8) (0x2fea)
- logger:// ----com.alexhay.logger (0x368c) (0x368e)
- auphd://---- com.adobe.hdcore (0x1734) (0x1736)
- scriptable://--------dk.simonbs.scriptable (0x3854) (0x3856)
- grammarly://-------- Grammarly Desktop Editor Protocol (0x3810) (0x3812)
- afp://----AFP URL (0x2fc8) (0x2fca) - [Apple Filing Protocol](https://developer.apple.com/library/archive/documentation/Networking/Conceptual/AFP/Introduction/Introduction.html#//apple_ref/doc/uid/TP40000854-CH1-SW1)
- apconfig://--------13132 (0x334c) (0x334e)
- apupdate://--------13132 (0x334c) (0x334e)
- dash-silent-open://----Dash-Silent-Open (0x1c68) (0x1c6a)
- stocks://----com.apple.stocks (0x32f0) (0x32f2)
- com.googleusercontent.apps.615390563111-q996sd7klo3509n959m03qrjo29trp32:// Cardhop (0x3570) (0x3572)
- photos-navigation://----Photos URL Handler (0x34d0) (0x34d2)
- dash-appcode://---- Dash-AppCode (0x1c58) (0x1c5a)
- photos://----Photos URL Handler (0x34d0) (0x34d2)
- itals://---- Live Stream URL (0x3100) (0x3102)
- macappstore://--------App Store URL (0x3500) (0x3502)
- x-maps-bulletin://----13468 (0x349c) (0x349e)
- dash-advanced://----Dash-Advanced (0x1c54) (0x1c56)
- itms-apps://--------App Store URL (0x3500) (0x3502)
- mapitem://--------13464 (0x3498) (0x349a)
- dash-plugin://--------Dash-Plugin (0x1c50) (0x1c52)
- x-cardhop://--------Cardhop (0x3570) (0x3572)
- textexpander://---- com.smileonmymac.textexpander.urlscheme6 (0x37f0) (0x37f2)
- web+textexpander://----com.smileonmymac.textexpander.urlscheme6 (0x37f0) (0x37f2)
- dash-advanced-with-keys://Dash-Advanced-With-Keys (0x1c48) (0x1c4a)
- marked://----URLHandlerMarked (0x3830) (0x3832)
- findmy://----com.apple.findmy (0x3108) (0x310a)
- findmyfriends://----com.apple.findmy (0x3108) (0x310a)
- grenada://--------com.apple.findmy (0x3108) (0x310a)
- dash-snippet://---- Dash-Snippet (0x1c64) (0x1c66)
- mhbookmarks://--------br.com.marcosatanaka.music-harbor (0x3688) (0x368a)
- mhalbum://--------br.com.marcosatanaka.music-harbor (0x3684) (0x3686)
- itms-bookss://--------iTunes Book Store URL (0x31a4) (0x31a6)
- fb://----Facebook (0x2ff0) (0x2ff2)
- itms-books://-------- iTunes Book Store URL (0x31a4) (0x31a6)
- maps://----13464 (0x3498) (0x349a)
- dash-workflow-callback://Dash-Workflow-Callback (0x1c60) (0x1c62)
- mhartist://--------br.com.marcosatanaka.music-harbor (0x3680) (0x3682)
- x-drafts://--------14040 (0x36d8) (0x36da)
- music://---- Music URL (0x30fc) (0x30fe)
- dict://----13084 (0x331c) (0x331e)
- musicharbor://--------br.com.marcosatanaka.music-harbor (0x367c) (0x367e)
- com.apple.tv://---- TV URL (0x3958) (0x395a)
- x-drafts-widget://----14040 (0x36d8) (0x36da)
- com.tapbots.tweetbot3mac.35700:// Tweetbot URL (0x38a0) (0x38a2)
- tweetbot.mac://---- Tweetbot URL (0x38a0) (0x38a2)
- com.googleusercontent.apps.894253971148-l0c4stqmtgbqe38m29eocvajjnn23eco:// 14040 (0x36d8) (0x36da)
- enpasslaunch://----in.sinew.Enpass-Desktop (0x3850) (0x3852)
- com.googleusercontent.apps.431426909032-ap08j302cl6tolmcgqpnhce0uutf8cg8:// 14040 (0x36d8) (0x36da)
- drafts5-callback-ignore://14040 (0x36d8) (0x36da)
- aem-asset://-------- com.adobe.aam (0x173c) (0x173e)
- drafts5-callback://----14040 (0x36d8) (0x36da)
- com.googleusercontent.apps.280246159890-6p3c2652mgdta3e721r877iqsip4skm1:// Fantastical (0x36a0) (0x36a2)
- x-drafts5-oauth://----14040 (0x36d8) (0x36da)
- https://---- Web site URL (0x37dc) (0x37de)
- x-fantastical3://----Fantastical (0x36a0) (0x36a2)
- x-dictionary://---- 13080 (0x3318) (0x331a)
- facetime-group://----FaceTime URL (0x3480) (0x3482)
- enpassauth://--------in.sinew.Enpass-Desktop (0x3850) (0x3852)
- x-drafts5://--------14040 (0x36d8) (0x36da)
- x-fantastical2://----Fantastical (0x36a0) (0x36a2)
- fmip1://---- com.apple.findmy (0x3108) (0x310a)
- drafts5://--------14040 (0x36d8) (0x36da)
- tg://----handler pref tg (0x3d4) (0x3d5), ru.keepcoder.Telegram (0x3694) (0x3696)
- enpass://----in.sinew.Enpass-Desktop (0x384c) (0x384e)
- pcast://---- Podcast Feed (0x32b8) (0x32ba)
- drafts://----14040 (0x36d8) (0x36da)
- com.tapbots.tweetbot3mac.store:// Tweetbot URL (0x38a0) (0x38a2)
- image2icon://-------- net.shinyfrog.image2icon.x-callback-url (0x355c) (0x355e)
- enpasscard://-------- in.sinew.Enpass-Desktop (0x3850) (0x3852)
- esse://----com.ameba.esse.open (0x3878) (0x387a)
- itms-services://----Store Services URL (0x3050) (0x3052)
- prefs://---- 14308 (0x37e4) (0x37e6)
- paste://---- com.wiheads.paste (0x37f4) (0x37f6)
- ssh://----ssh URL (0x336c) (0x336e)
- dash-feed://--------Dash-Feed (0x1c5c) (0x1c5e)
- daap://----Remote Library URL (0x30f8) (0x30fa), Remote Library URL (0x3954) (0x3956)
- itvls://---- Live Stream URL (0x395c) (0x395e)
- facetime-audio://----FaceTime URL (0x3480) (0x3482)
- enpassstart://--------in.sinew.Enpass-Desktop (0x3850) (0x3852)
- com.googleusercontent.apps.639604012593-s8nrj1rbjoa8ajhoksm01fs2gqmpq6ks:// 14040 (0x36d8) (0x36da)
- ftps://----FTPS URL (0x3774) (0x3776)
- cifs://----SMB URL (0x2fd4) (0x2fd6)
- noir://----nl.jeffreykuiken.NoirApp (0x38a4) (0x38a6)
- macappstores://---- App Store URL (0x3500) (0x3502)
- dash://----Dash (0x1c4c) (0x1c4e)
- ipp://----AirPrint (0x2fe8) (0x2fea)
- x-fantastical://----Fantastical (0x36a0) (0x36a2)
- applefeedback://----com.apple.appleseed.FeedbackAssistant.action (0x3034) (0x3036)
- sftp://----SFTP URL (0x3778) (0x377a)
- itms-appss://-------- App Store URL (0x3500) (0x3502)
- x-maps-mapitemhandles://13464 (0x3498) (0x349a)
- messages://--------Messages URL (0x34e8) (0x34ea)
- lookupapp://--------in.muditbhargava.lookup (0x36e0) (0x36e2)
- taio://----app.cyan.taio (0x38d4) (0x38d6)
- tweetbot://--------Tweetbot URL (0x38a0) (0x38a2)
- shareful://--------14316 (0x37ec) (0x37ee)
- shortcuts://--------is.workflow.app.url-scheme (0x3490) (0x3492)
- rniomacsafari://----io.raindrop.safari.scheme (0x3554) (0x3556)
- com.tapbots.tweetbot3mac://Tweetbot URL (0x38a0) (0x38a2)
- shortcuts-production:// is.workflow.app.url-scheme (0x3490) (0x3492)
- ibooks://----iTunes Book URL (0x31a8) (0x31aa)
- fe://----com.skyjos.mac.fileexplorer (0x36dc) (0x36de)
- videos://----TV URL (0x3958) (0x395a)
- aam://----com.adobe.aam (0x173c) (0x173e)
- itms-beta://--------com.apple.TestFlight.scheme (0x3690) (0x3692)
- com.agiletortoise.drafts5://14040 (0x36d8) (0x36da)
- itmss://---- Music URL (0x30fc) (0x30fe)
- fmf1://----com.apple.findmy (0x3108) (0x310a)
- bluetoothinspector://---- 14356 (0x3814) (0x3816)
- smb://----SMB URL (0x2fd4) (0x2fd6)
- x-github-client://----handler pref x-github-client (0x3e8) (0x3e9), com.github.GitHubClient (0x381c) (0x381e)
- com.googleusercontent.apps.875066922361-71vgg0cfpkhgmlgfmgnevpcrraggpid0:// Fantastical (0x36a0) (0x36a2)
- userscriptsurlscheme:// com.userscripts.macos (0x3880) (0x3882)
- one-thing://--------com.sindresorhus.One-Thing (0x3b00) (0x3b02)
- telegram://--------ru.keepcoder.Telegram (0x3694) (0x3696)
- itms-podcasts://----Podcast Feed (0x32b8) (0x32ba)
- otpauth://--------System Preferences URL (0x3544) (0x3546)
- itsradio://--------Radio URL (0x3104) (0x3106)
- map://----13464 (0x3498) (0x349a)
- podcast://--------Podcast Feed (0x32b8) (0x32ba)
- com.googleusercontent.apps.588137298651-ds3aivu0ai0jfaumcsfu0773fhrdo5ji:// 13668 (0x3564) (0x3566)
- x-apple.systempreferences://System Preferences URL (0x3544) (0x3546)
- x-maps-ac-auth://----13460 (0x3494) (0x3496)
- itlss://---- Live Stream URL (0x3100) (0x3102), Live Stream URL (0x395c) (0x395e)
- facetime-open-link://---- FaceTime URL (0x3480) (0x3482)
- workflow://--------is.workflow.app.url-scheme (0x3490) (0x3492)
- cloudkit-7adb8cc6tf.in.sinew.walletx:// in.sinew.Enpass-Desktop (0x3850) (0x3852)
- tel://----FaceTime URL (0x3480) (0x3482)
- x-apple-reminderkit://----ReminderKit (0x34f4) (0x34f6)
- applenewss://-------- com.apple.NewsCustomScheme (0x3dac) (0x3dae)
- ical://----iCal URL (0x352c) (0x352e)
- ichat://---- iChat URL (0x34e4) (0x34e6)
- podcasts://--------Podcast Spotlight (0x32bc) (0x32be)
- tot://----Tot URL scheme (0x388c) (0x388e)
- file://----File URL (0x2fcc) (0x2fce), Local file URL (0x37e0) (0x37e2)
- jayson://----dk.simonbs.Jayson (0x3888) (0x388a)
- imessage://--------IMSG (0x34e0) (0x34e2)
- hp-jarvis-auth-harness-mac-oauth2:// com.HP.Jarvis.WebView.Reference.MacOS (0x3568) (0x356a)
- apple-otpauth://----System Preferences URL (0x3544) (0x3546)
- facetime://--------handler pref facetime (0x424) (0x425), FaceTime URL (0x3480) (0x3482)
- applenews://--------com.apple.NewsCustomScheme (0x3dac) (0x3dae)
- itunesradio://--------Radio URL (0x3104) (0x3106)
- telnet://----telnet URL (0x3368) (0x336a)
- itms-messagess://----Message Store URL (0x34dc) (0x34de)
- postman://--------postman (0x3780) (0x3782)
- musics://----Music URL (0x30fc) (0x30fe)
- github-mac://-------- handler pref github-mac (0x410) (0x411), com.github.GitHubClient (0x381c) (0x381e)
- dash-install://---- Dash-Install (0x1c6c) (0x1c6e)
- simplenote://-------- 13992 (0x36a8) (0x36aa)
- x-apple-tips://---- 12164 (0x2f84) (0x2f86)
- mailto://----Email Address URL (0x3310) (0x3312)
- nwnode://----NWNode URL (0x2fd8) (0x2fda)
- sms-private://--------SMS Private URL (0x34d8) (0x34da)
- x-man-page://-------- x-man-page URL (0x3370) (0x3372)
- x-marked://--------URLHandlerMarked (0x3830) (0x3832)
- http://----Web site URL (0x37dc) (0x37de)
- notes://---- com.apple.Notes (0x31d4) (0x31d6)
- grammarly.extension://----com.grammarly.safari.extension (0x3784) (0x3786)
- im://----CPIM (0x34ec) (0x34ee)
- webcal://----Remote Calendar URL (0x3528) (0x352a), Subscribe to calendar (0x36a4) (0x36a6)
- itms-messages://----Message Store URL (0x34dc) (0x34de)
- itms://----Music URL (0x30fc) (0x30fe)
- httpbot://--------httpbot (0x377c) (0x377e)
- com.fantastical.oauth://Fantastical (0x36a0) (0x36a2)
- psdr-mntr://--------com.hp.PSDrMonitor.url-scheme (0x16c4) (0x16c6)
- sms://----SMS URL (0x34d4) (0x34d6)
- message://--------Email Message Storage URL (0x3314) (0x3316)
- ftp://----FTP URL (0x2fd0) (0x2fd2), FTP URL (0x3770) (0x3772)
- addressbook://--------Contacts URL (0x3340) (0x3342)
- snippetslab://--------com.renfei.SnippetsLab (0x3c64) (0x3c66)
- hp-smart-mac-oauth2://----com.hp.SmartMac (0x3560) (0x3562)
- highlightsapp://----com.finnvoorhees.Highlights (0x3834) (0x3836)
- gladys://----build.bru.Gladys (0x3844) (0x3846)
- cloudphoto://--------Photos URL Handler (0x34d0) (0x34d2)
- help://----12164 (0x2f84) (0x2f86)
- italss://----Live Stream URL (0x3100) (0x3102)
- itls://----Live Stream URL (0x3100) (0x3102), Live Stream URL (0x395c) (0x395e)
- itvlss://----Live Stream URL (0x395c) (0x395e)
- itunes://----Music URL (0x30fc) (0x30fe)
- com.apple.watchlist://----TV URL (0x3958) (0x395a)
- twitter://--------Twitter (0x2fec) (0x2fee)
- x-bunch://--------Bunch Protocol (0x3550) (0x3552)
- com.fantastical.meetup.oauth:// Fantastical (0x36a0) (0x36a2)
- x-github-desktop-auth://handler pref x-github-desktop-auth (0x3fc) (0x3fd), com.github.GitHubClient (0x381c) (0x381e)