---
{"dg-publish":true,"permalink":"/snippets/sort-all-directories-based-on-their-si/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Sort all directories based on their size
Updated `09042022-082835`

- [Drafts](drafts://open?uuid=CAABBB06-186C-437D-BC30-65844BDBEC2B)
- [WTF](https://davidblue.wtf/drafts/CAABBB06-186C-437D-BC30-65844BDBEC2B.html)
- Simplenote Local
- Simplenote Publish

---

du -sh -- *  | sort -rh  # Files and directories, or
du -sh -- */ | sort -rh  # Directories only

```
du -sh -- *  | sort -rh  # Files and directories, or
du -sh -- */ | sort -rh  # Directories only
```

---

## Hex

6475202d7368202d2d202a20207c20736f7274202d7268



Tags:
  cli, documentation, files, linux, reference, simplenote, snippets, stack, ~