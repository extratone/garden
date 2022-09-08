---
{"dg-publish":true,"permalink":"/snippets/big-sur-subject-field/","dgHomeLink":true,"dgPassFrontmatter":false}
---

big-sur-subject-field

---
created: 2022-01-15T15:52:18Z
folder: Gist
gist: https://gist.github.com/af338a136e3580000636fa3cc89f4488
language: Markdown
modified: 2022-01-15T15:52:18Z
notes: |
    Enable iMessage (Messages) Subject Field in macOS Big Sur
    Author: extratone (https://gist.github.com/af338a136e3580000636fa3cc89f4488)
title: big-sur-subject-field.md
---

Want the Subject field (for bold iMessages) in macOS Big Sur's Messages app?

1. Quit Messages
1. Open Terminal
1. Run `defaults write com.apple.MobileSMS MMSShowSubject 1`
1. Start Messages