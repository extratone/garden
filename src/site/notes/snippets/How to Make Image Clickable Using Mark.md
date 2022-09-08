---
{"dg-publish":true,"permalink":"/snippets/how-to-make-image-clickable-using-mark/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# How to Make Image Clickable Using Markdown?
Updated `08162022-125602`

- [**How to Make Image Clickable Using Markdown?**](https://devblog.dinobansigan.com/how-to-make-image-clickable-using-markdown) | *Attach to Process*
- [WTF](https://davidblue.wtf/drafts/CAABBB06-186C-437D-BC30-65844BDBEC2B.html)
- Simplenote Local
- Simplenote Publish
- Things

---

For awhile now, I was wondering if it was possible to use Markdown, to make an image clickable. By that I mean, display an image in a blog post, and allow the reader to click that image to view the image in a tab. *You can see an example at the end of this post.*

So anyway, I know what the Markdown syntax is for a link and for an image, but I've never been able to put the two together until today. 

*Thanks to [this post](https://firepress.org/en/how-to-make-an-image-clickable-with-markdown/) for the idea on how to do it. This saved me from having to write JavaScript that would find all the Snap.as images in a blog post, then wrap them in an `<a></a>` tag just to make the images clickable and open in a browser tab.*

So just to recap, the Markdown syntax for a link is this:

`[Link text](Link URL)`

And the Markdown syntax for an image is this:

`![Alt Text for image](Image URL)`

So, given the Markdown listed below for an image, how do you display the image and make it clickable at the same time?

`![Mazda FC RX-7 - A little drifting action](https://i.snap.as/2IxnDguK.png)`

The answer is that you put the Markdown for the image inside the Markdown for a link, like so:

`[![Mazda FC RX-7 - A little drifting action](https://i.snap.as/2IxnDguK.png)](https://i.snap.as/2IxnDguK.png)`

A couple of things to note here:

- The whole Markdown for the image goes inside the brackets `[]`, the "Link text" portion of the Markdown for a link. This is what allows the image to show up as the content of a link.
- The URL to the image goes inside the parenthesis `()`, the "Link URL" portion of the Markdown for a link. It kinda looks redundant, having the same URL to the image one after another. But that's how you make it work with the Markdown syntax for an image and a link.

And finally, here it is in action:

[![Mazda FC RX-7 - A little drifting action](https://i.snap.as/2IxnDguK.png)](https://i.snap.as/2IxnDguK.png)



Tags:
  as, documentation, md, reference, simplenote, snippets