---
{"dg-publish":true,"permalink":"/snippets/accessing-a-shortcut-s-metadata/","dgHomeLink":true,"dgPassFrontmatter":false}
---

Accessing a shortcut's metadata

---
created: 2022-03-20T23:30:10Z
folder: Shortcuts
language: Markdown
modified: 2022-03-20T23:39:16Z
notes: [atnbueno/shortcut-icons: CSS sprite to represent iOS shortcut icons](https://github.com/atnbueno/shortcut-icons)
tags: shortcuts, dev, json
title: Accessing a shortcut's metadata
---

# shortcut-icons

A CSS sprite to represent iOS shortcut icons.

Grab the [stylesheet](https://github.com/atnbueno/shortcut-icons/blob/main/shortcut-icons.css) and the [default (iOS 15) glyph set](https://github.com/atnbueno/shortcut-icons/blob/main/ios15-glyphs.png), and add a shortcut icon to your HTML with just an empty `div` element:

```html
<div class="shortcut-icon c4251333119 g59793 s86"></div>
```

In this example `shortcut-icon` is the base CSS class. The secondary `c4251333119` class is the orange **color** from iOS 15, the `g59793` class is the "paintbrush" **glyph** and the `s86` class is the desired **icon size**. See the [demo.html](https://github.com/atnbueno/shortcut-icons/blob/main/demo.html) file for more examples./Users/blue/Library/Mobile Documents/com~apple~CloudDocs/Family

The color and glyph **numeric values** can be found both in the shortcut metadata (see below) and in its _plist_ (the shortcut "source code").

The HTML element doesn't have to be a `<div>`, although using other elements may require additional CSS to reset their appearance.

If you want to use the colors and glyphs from iOS 12-14, grab the glyph sets you want to use and add an additional `ios12`, `ios13`, or `ios14` class to each HTML element.

And if you need a size not in the CSS, it's easy to define your own. For example, to get 58×58 icons:

```css
.s58  { --icon-size:  58px }
```

## Accessing a shortcut's metadata

To access a shortcut's metadata add `api/records/` after `shortcuts/` in its iCloud link. Example:

<https://www.icloud.com/shortcuts/0e011689efc949a291f231333c6dd2b3> \
↓\
<https://www.icloud.com/shortcuts/api/records/0e011689efc949a291f231333c6dd2b3>

## Sites that use this

- [RoutineHub](https://routinehub.co/)
- My (non-public yet 😅) website