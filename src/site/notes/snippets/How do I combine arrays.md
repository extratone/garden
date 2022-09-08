---
{"dg-publish":true,"permalink":"/snippets/how-do-i-combine-arrays/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# How do I combine arrays?

---



There are many ways to combine arrays. One way is to use the + operator:

var a = [1, 2, 3]; var b = [4, 5, 6]; var c = a + b; // [1, 2, 3, 4, 5, 6]

Another way is to use the Array.concat() method:

var a = [1, 2, 3]; var b = [4, 5, 6]; var c = a.concat(b); // [1, 2, 3, 4, 5, 6]

If you want to combine arrays and create a new array without modifying the original arrays, you can use the Array.prototype.concat() method:

var a = [1, 2, 3]; var b = [4, 5, 6]; var c = a.concat(b); // [1, 2, 3, 4, 5, 6

Tags:
  js