---
title: Snap.as/Write.as API
tags: reference, writeas, snippets, documentation, cli
davodtime: 09082022-105545
local: shareddocuments:///private/var/mobile/Library/Mobile%20Documents/iCloud~md~obsidian/Documents/OBSHIDDIAN/drafts/BD1C9DBB-3C89-4FD9-AC9F-4D43BF2C7F08.md
dg-publish: true
share: true
draft: drafts://open?uuid=BD1C9DBB-3C89-4FD9-AC9F-4D43BF2C7F08
---

curl "https://snap.as/api/photos/upload" \
  -H "Authorization: 00000000-0000-0000-0000-000000000000" \
  -F "file=@photo.jpeg"

curl "https://snap.as/api/photos/upload" \
  -H "Authorization: 08676b98-947f-4dbe-47e6-74c244e9a32b" \
  -F "file=@photo.jpeg"

curl "https://write.as/api/auth/login" -H "Content-Type: application/json" -X POST -d '{"alias": "extratone", "pass": "ytAcBvZRNIx-YQlO0j3z?dxPEfc"4hKZm"}'

curl "https://write.as/api/auth/login" \
  -H "Content-Type: application/json" \
  -X POST \
  -d '{"alias": "extratone", "pass": "zpH2TV9FR9DxvAfg"}'


curl "https://write.as/api/markdown" -H "Content-Type: application/json" -X POST -d '{"raw_body": "This is *formatted* in __Markdown__."}'

curl "https://write.as/api/posts" -H "Content-Type: application/json" -X POST -d '{"body": "Testing", "title": "My First Post"}’
08676b98-947f-4dbe-47e6-74c244e9a32b

curl "https://snap.as/api/me/photos" \
  -H "Authorization: 08676b98-947f-4dbe-47e6-74c244e9a32b"

curl "https://snap.as/api/me/photos" -H "Authorization: 08676b98-947f-4dbe-47e6-74c244e9a32b" | pbcopy

08676b98-947f-4dbe-47e6-74c244e9a32b