---
{"dg-publish":true,"permalink":"/snippets/path-finder-new-browser-js/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# PathFinderNewBrowser.js

- [applescripts/Path Finder New Browser.javascript at main · kotfu/applescripts](https://github.com/kotfu/applescripts/blob/main/src/Path%20Finder%20New%20Browser.javascript)

---
#!/usr/bin/env osascript -l JavaScript
/*
a script to open a new Path Finder window

This script exists so that I can do it from LaunchBar
*/

var pf = Application('System Events').processes.byName('Path Finder');

pf.menuBars[0].menuBarItems.byName('File').menus[0].menuItems.byName('New Browser').menus[0].menuItems.byName('New Browser').click();

Tags:
  js, legacy, macos, snippets