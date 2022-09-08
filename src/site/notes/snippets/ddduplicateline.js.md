---
{"dg-publish":true,"permalink":"/snippets/ddduplicateline-js/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# ddduplicateline.js

- [Action Directory](https://actions.getdrafts.com/a/2B8)

---
```js
// grab ranges and text
let [selStart, selLen] = editor.getSelectedRange()
let [lnStart, lnLen] = editor.getSelectedLineRange()
let lnText = editor.getTextInRange(lnStart, lnLen)
let flNeedsLineFeed = !lnText.endsWith("\n") 

// insert duplicate of current line below it
editor.setTextInRange(lnStart + lnLen, 0, `${flNeedsLineFeed ? "\n" : ""}${lnText}`)
```

Tags:
  actions, drafts, js, snippets, text