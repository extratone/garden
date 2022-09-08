---
{"dg-publish":true,"permalink":"/snippets/i-message-url-scheme/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# iMessage URL Scheme

- [Start an iMessage Conversation from the web with Custom Links](https://osxdaily.com/2012/05/15/start-an-imessage-conversation-from-the-web-with-custom-links/) | *OSX Daily*

---
By using a custom URL inside of an anchor tag, you can place a link on any website that will initiate a new iMessage conversation. Anyone clicking the link will then launch the Messages app in iOS or iMessages in Mac OS X to begin a new conversation with the specified Apple ID.

Even if you have limited knowledge of HTML the link structure is easy to use, here’s the format you’d want to use for Mac and iOS;

Mac OS X: `imessage://your@appleid.com`

`<a href="imessage://your@appleid.com">Send iMessage to a Mac</a>`

iOS: `sms://your@appleid.com`

`<a href="sms://your@appleid.com">Send iMessage to iOS</a>`

Replace “your@appleid.com” with your own Apple ID that is configured to use with iMessage. Note that the iOS link uses “sms” as the identifier, meaning some users may send you an actual text message rather than iMessage if they are not set up to use Apple’s messaging protocol.

Because iOS and OS X use different URL schemes, you’ll need to use two different links by default. This could have advantages, if you only wanted people from iOS to reach you for example, but if you don’t like that idea there’s a nice workaround to the dual links by using the short PHP script offered by Beuagil.es. This script will detect the user agent and determine which link to use based on that, effectively combining the two iMessage links into one intelligent link:

```
<a href="<?php
$useragent = $_SERVER['HTTP_USER_AGENT'];
if(preg_match('/Macintosh/',$useragent)) $os = 'imessage';
elseif(preg_match('/iPhone/',$useragent)) $os = 'sms';
else $os = 'sms';
echo $os;
?>:your@appleid.com">Send an iMessage</a>
```

Obviously you’ll need a PHP capable website for the above script to work, otherwise you’ll have to use the HTML snippets offered at the top of the post.

Tags:
  imessage, sms, snippets, url, x