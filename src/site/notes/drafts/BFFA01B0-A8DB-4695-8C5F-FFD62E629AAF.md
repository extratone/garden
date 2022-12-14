---
title: Tot Guide
tags: macos, birthday, documentation
davodtime: 09082022-105601
local: shareddocuments:///private/var/mobile/Library/Mobile%20Documents/iCloud~md~obsidian/Documents/OBSHIDDIAN/drafts/BFFA01B0-A8DB-4695-8C5F-FFD62E629AAF.md
dg-publish: true
share: true
draft: drafts://open?uuid=BFFA01B0-A8DB-4695-8C5F-FFD62E629AAF
---

## Make Tot your own.

At the top-right of Tot’s window there is a toggle for settings. Here are some things that you can do to make the app fit your workflow:

_Use a menu bar icon with a detachable window:_ With this setting, the window is tucked away at the top of your screen, but you can drag it away when needed. With this setting, there is no _Dock_ icon or application menu so this is where you can quit the app.

_Appearance:_ Tot looks great whether you prefer a dark or light interface. And you’ll either love or hate the colored background, so make your choice!

_Set a system-wide hotkey:_ This setting allows Tot to become a keyboard-only app: the key combination you specify will bring up the window and allow you to type or navigate with keyboard shortcuts.

In addition to the settings view, you can also configure Tot using the menu bar:

_Style the text view:_ The font for both rich and plain text can be customized along with the size and tab spacing using _Format_ in the menu bar or from the context menu while you’re editing text.

_Configure the text view:_ Sometimes smart quotes are just what you need, sometimes they screw up your code. Use the _Edit_ > _Substitions_ and _Spelling and Grammar_ menus to tweak the text view to your needs. Each dot has its own settings and they are synced to other devices. (They are currently unused on iOS because there's no standard way to modify the settings there.)

_Floating window:_ When you're taking notes, it can be helpful to have Tot's window above all others. Use _Window_ > _Display as Floating Window_ and the window will always be visible and ready to go!

And speaking of menus, if you find an item with a keyboard combo that you don't like (switching tabs!), take a look at our [handy guide for customizing shortcuts](https://support.iconfactory.com/kb/tot/keyboard-shortcuts-in-tot).



**Tot loves links.**

Whether you’re in plain text or rich text, Tot handles links intelligently. If you drag a link from a web browser, you’ll get the page title and URL formatted as rich text or as Markdown inline link. In plain text mode, it’s easy to edit the parts individually; rich text gives you a clickable link.

This conversion also happens if you copy and paste a block of text from a web page: text and links are converted on the fly. If you’re entering URLs manually, they’ll automatically be detected as you type.

Links aren’t limited to just web pages. [Click here](dict://tot) to see "tot" in the dictionary. Here are other useful examples:

<dict://CHOCK>
<x-bbedit://open?url=file:///etc/hosts>
<facetime:18005551212>
<tel:1-800-555-1212>
<ssh://root@example.com>

Try dragging a message from Mail into Tot’s window: you will get [a link](https://daringfireball.net/2007/12/message_urls_leopard_mail) that’s a simple way to reference conversations and other information!

Finally, Tot has its own URL scheme that can automate tasks. It works like this:

tot:// + _host_ + _operation_ + ? + _parameter_

The _host_ is "1" to "7" and will open the numbered dot (left to right). If you specify "empty", the first empty dot is selected. Use "settings" and "help" to open their views.

The _operation_ can be specified for dots; use "/prepend" to insert text at the beginning, "/append" to add to the end, or "/replace" the entire contents of dot. The _parameter_ is "text" and a URL encoded string. For example, <tot://1/append?text=odds+%26+ends%0A> will add some text to the end of the first dot. To open the first dot from the Terminal, use _open_ and this URL:

$ open tot://1

If you’re using the scheme from an AppleScript, "/content" will return the text from the selected dot. Try this:

$ osascript -e 'tell application "Tot" to open location "tot://6/content"'

There is no support for rich text in the URL scheme: use Markdown in plain text to get formatting. If this functionality appeals to you, look at [this shell script](https://gist.github.com/chockenberry/d33ef5b6e6da4a3e4aa9b07b093d3c23).
