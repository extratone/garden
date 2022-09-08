---
{"dg-publish":true,"permalink":"/snippets/ddrop-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

ddrop (2)

---
created: 2020-12-04T13:00:30Z
folder: Gist
gist: https://gist.github.com/47e45b6a7f30738d66a0774e7f1eea0b
language: Markdown
modified: 2020-12-04T13:00:30Z
notes: |
    How to convert a list of URLs to a bookmarks.html file.
    Author: extratone (https://gist.github.com/47e45b6a7f30738d66a0774e7f1eea0b)
title: ddrop.md
---

# Discord Channel Links to Raindrop Bookmarks

## How to Migrate Links in Discord Channels to Raindrop Collections

# The Dilemma

I have used [a Discord channel](https://discord.gg/4hdQcVd) as my "Reading List" for years, but have been using [Raindrop](https://raindrop.io/) in the past month and would like to migrate all the links to all the articles, essays, videos, etc that I've posted in the channel through its existence into my [Reading List Collection](https://raindrop.io/collection/13380406) on Raindrop.

# Requisites

- The [Discord Chat Exporter](https://github.com/Tyrrrz/DiscordChatExporter/releases).
- This [URL Extrator Tool](https://www.convertcsv.com/url-extractor.htm)
- This [Bookmark HTML File Generator](https://atkinsio.com/bookmarks-html-generator/)

---

# Process

1. Using the [Discord Chat Exporter](https://github.com/Tyrrrz/DiscordChatExporter/releases) tool, export your desired Discord channel's content in **CSV format**.
2. Using this online [URL Extractor Tool](https://www.convertcsv.com/url-extractor.htm), upload the CSV file and extract URLS from it.
3. Copy the extracted raw list of URLs.
4. Paste the URLs into the input of this [Bookmark HTML File Generator](https://atkinsio.com/bookmarks-html-generator/) and select "Download Bookmarks."
5. In Raindrop's import interface, select the HTML file you download to import.