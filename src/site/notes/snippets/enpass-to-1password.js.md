---
{"dg-publish":true,"permalink":"/snippets/enpass-to-1password-js/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# enpass-to-1password.js

---
const fs = require('fs'); const args = process.argv; const inputFile = args[2] || 'vault.json'; const outputFile = args[3] || 'vault.csv'; console.log('\nREADING: ' + inputFile + '\n'); try { const contents = fs.readFileSync(inputFile); const vault = JSON.parse(contents); let notConverted = 0; let converted = 0; const csvOutput = ['title,website,username,password,notes,category']; const fieldMapping = { title: 'title', url: 'website', username: 'username', password: 'password', notes: 'notes', category: 'category' }; vault.items.forEach(item => { if ( item.category === 'login' || item.category === 'password' || item.category === 'uncategorized' ) { const rowData = { title: item.title, website: '', username: '', password: '', notes: item.note, category: item.category }; Object.keys(fieldMapping).forEach(type => { const key = fieldMapping[type]; if (item.fields !== undefined) { item.fields.forEach(field => { if (field.type === type) { if (field.value 

Tags:
  1, cli, conversion, enpass, js, obfuscation, snippets