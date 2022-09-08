---
{"dg-publish":true,"permalink":"/snippets/custom-drafts-tags/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Custom Drafts Tags

- [Custom Tags](https://docs.getdrafts.com/docs/actions/templates/drafts-templates#custom-tags)

---
# Custom Tags  In addition to the predefined tags always available, scripts in an action can create custom tags which become available to action steps run after the script in the same action. This is useful if a scripted action step processes text to create a value that then needs to be inserted in a later step that shares that text. The below example shows a simple script with creates a tag.

```js let s = "My String Value"; draft.setTemplateTag("mytag", s); // after running this script, templates later // in the action will have available a [[mytag|mytag]] tag.
```
 Custom template tag values can also be created using the Define Template Tag action step


Tags:
  automation, drafts, js, snippets, template