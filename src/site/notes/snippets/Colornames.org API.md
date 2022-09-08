---
{"dg-publish":true,"permalink":"/snippets/colornames-org-api/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Colornames.org API
Updated `07212022-135614`

- [Original Reference](https://colornames.org/download/)
- [WTF](https://davidblue.wtf/drafts/CB53592F-F12F-461E-8F6A-A94992749AA9.html)
- Simplenote Local
- Simplenote Publish
- Things
---

**JSON feed of the latest 100 submissions:**  
`https://colornames.org/fresh/json/`

Returns:  
`[{"nameId":1944061,"hexCode":"4c72f2","name":"Roneria"},{"nameId":1944060,"hexCode":"7ce0ef","name":"Puffy"}, ... ]`

---

**JSON lookup of hex to color name:**
`https://colornames.org/search/json/?hex=00006B`

Returns:  
`{"hexCode":"00006b","name":"David Blue"}`

---

**JSON request for a random color name:**
`https://colornames.org/random/json/`

Returns:  
`{"hexCode":"f7ff85","name":"Panic Urine"}`

Tags:
  api, colors, hex, reference, snippets