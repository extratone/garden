---
{"dg-publish":true,"permalink":"/snippets/legacy-docsets-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

LegacyDocsets (2)

---
created: 2021-05-02T08:15:39Z
folder: Gist
gist: https://gist.github.com/0dec1e6ac15bd2716a5e114aa4c20c0c
language: Markdown
modified: 2021-05-02T08:15:39Z
notes: |
    Download and view old Apple developer documentation
    Author: extratone (https://gist.github.com/0dec1e6ac15bd2716a5e114aa4c20c0c)
title: LegacyDocsets.md
---

# How to download and view legacy documentation from Apple (no need to sign in to your dev account)

1. Download the [docset index XML](https://developer.apple.com/library/downloads/docset-index.dvtdownloadableindex).
2. Find the docset you want (there are some with URL https://apple.com/none.dmg; ignore them - you will find them again further down the file with a working URL).
3. Download the dmg. It's probably around a gigabyte or so.
4. "Install" the .pkg file somewhere on your disk. If you don't trust the installer, do it manually:
   1. Find the largest file, named Payload, and extract it using The Unarchiver.
   2. This creates a new, even larger file, probably named Payload-1.
   3. Extract Payload-1 using The Unarchiver.
5. After many minutes of extracting, we have our .docset file.
6. Use Kapeli Dash to browse and read the docset.

Why? Because Apple's old docs are often more verbose, and because they didn't mix iOS and macOS docs into one big mess. Or just because you need good information for backward compatibility, or what the official word was back in time.