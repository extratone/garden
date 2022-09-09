---
{"dg-publish":true,"permalink":"/drafts/a9-a8-e5-ba-a7-bb-4-ddb-a62-f-018-a84-c93-b8-b/","dgHomeLink":true,"dgPassFrontmatter":false}
---

Updated `08162022-132527`

- [**Attach to Process Write.as Theme**](https://devblog.dinobansigan.com/attach-to-process-write-as-theme)
- [WTF](https://davidblue.wtf/drafts/CAABBB06-186C-437D-BC30-65844BDBEC2B.html)
- [Simplenote Local](simplenote://note/1689ec7b4852457192cef3508ad17a72)
- [Simplenote Publish](http://simp.ly/publish/4C4ZCM)
- [Things](things:///show?id=SVVfZoNtW7pqsQnUgtXeEQ)

---

```css
/* Written in 2020 by Riley Walz

 This theme is licensed under a Creative Commons Attribution 4.0 
 International License.

 You should have received a copy of the license along with this
 work. If not, see http://creativecommons.org/licenses/by/4.0/
*/

.post-title {
    padding-right: 1em;
}

.book {
	display: none;
}

.read-more {
	display: none;
}

.h-entry {
	justify-content: space-between;
	display: flex;
}

body#collection #wrapper article,
body#subpage #wrapper article {
	margin-bottom: 1em;
}

.dt-published {
	flex-shrink: 0;
}

@media screen and (max-width: 700px) {
	.h-entry {
		display: block
	}
	body#collection #wrapper time,
	body#subpage #wrapper time {
		font-size: 0.9em;
	}
	.post-title {
		font-size: 1.2rem;
	}
	body#collection #wrapper article,
	body#subpage #wrapper article {
		margin-bottom: 1.5em;
	}
}

#emailsub {
	text-align: center;
	margin-top: 50px;
}

/*** My own theme changes ***/
#post article {
    max-width: 60rem;
}

body#post header, body#subpage header {
	margin-bottom: 1em;
}

body#post header h1 {
    font-size: 2em;
}

body#post pre {
    margin-bottom: -2.5em;
}

#post-body div.e-content div.contact-form {
    display: contents;
    margin-top: -3em;
}

#fnContactEmbed {
    display: none;
}

#fnContactEmbedIframe {
	background: #FAFAD2;
	border-radius: 6px;
}

/* Dark Theme attempt */
body {
    font-family: Inter,-apple-system,BlinkMacSystemFont,Roboto,Segoe UI,Helvetica,Arial,sans-serif!important;
    text-rendering: optimizeLegibility;
    -webkit-text-size-adjust: 100%;
    
    background: #292a2d;
    /*background-secondary: #3b3d42;
    header: #252627;*/
    color: #a9a9b3;
    /*color-secondary: #73747b;*/
    border-color: #4a4b50;
}
#post article.norm, .font.norm, body#collection article.norm, body#subpage article.norm, input#title.norm, pre.norm, span.norm, textarea.norm {
    font-family: Inter,-apple-system,BlinkMacSystemFont,Roboto,Segoe UI,Helvetica,Arial,sans-serif!important;
}
#post nav a:not(.home), header nav a {
    color: #a9a9b3;
}

body h1 a, body header h2 a, header p.description, .post-title a:link, .post-title a:visited, a, a:visited {
    color: #a9a9b3;
}
body h1 a:hover, body header h2 a:hover, div.e-content p a, div.e-content ul li a {
    color: #a9a9b3;
    text-decoration: underline;
}
body#post article time.dt-published, body#subpage article time.dt-published {
    color: #73747b;
}

#subscribe-btn {
    border: 1px #045FB4;
    background: #045FB4;
}
#subscribe-btn:hover {
    text-shadow: 0px 0px 6px white;
}

.e-content a.hashtag:link {
    background-color: #292a2d;
    border-radius: 7px;
    border-style: solid;
    border-color: #a9a9b3;
    border-width: 1px;
    padding-left: 10px;
    padding-right: 10px;
    padding-top: 2px;
    padding-bottom: 2px;
    text-decoration: none;
	font-style: normal;
    line-height: 2em;
    color: #a9a9b3;
}
.e-content a.hashtag:visited {
    color: #a9a9b3;
	text-decoration: none;
}
.e-content a.hashtag:hover span + span {
    text-decoration: none;
}
.e-content a.hashtag:hover {
    background-color: #a9a9b3;
    border-color: #a9a9b3;
    color: #292a2d;
    text-decoration: none;
}

body footer {
    text-align: center;
    padding: 0 2em;
}

body footer nav {
    color: #73747b;
    padding-bottom: 48px;
    margin-bottom: 0px;
}

body footer nav a {
    font-weight: bold;
    color: #73747b!important;
    text-decoration: none!important;
    margin: 0!important;
}
body footer nav a:hover {
    color: #a9a9b3!important;
    text-decoration: underline!important;
    margin: 0!important;
}

body #post code, body#collection code, body#post code, body#subpage code {
	font-family: Consolas,Monaco,Andale Mono,Ubuntu Mono,monospace;
	background: #282c34;
	border-color: #3b3d42;
	padding: 3px 6px 3px 6px;
	margin: 0 2px;
	border-radius: 5px;
	font-size: .9rem;
	font-weight: 400;
}
body #post pre, body#collection pre, body#post pre, body#subpage pre {
    background: #282c34;
    border: 1px solid #3b3d42;
}

#hyvor-talk-view {
    margin-top: 1em;
    margin-bottom: -4em;
}

/* Hide post views */
header nav .views {
    display: none;
}

/* Hide Stats link */
nav#manage ul a[href="/me/c/attach-to-process/stats"],
nav#manage ul a[href="/me/c/attach-to-process/subscribers"]{
  display: none;
}

/* Highlight.js Atom One Dark Reasonable Theme */
.hljs {
	display: block!important;
	overflow-x: auto!important;
	padding: .5em!important;
	color: #abb2bf!important;
	background: #282c34!important;
}

.hljs-keyword,
.hljs-operator {
	color: #f92672!important;
}

.hljs-pattern-match {
	color: #f92672!important;
}

.hljs-pattern-match .hljs-constructor {
	color: #61aeee!important;
}

.hljs-function {
	color: #61aeee!important;
}

.hljs-function .hljs-params {
	color: #a6e22e!important;
}

.hljs-function .hljs-params .hljs-typing {
	color: #fd971f!important;
}

.hljs-module-access .hljs-module {
	color: #7e57c2!important;
}

.hljs-constructor {
	color: #e2b93d!important;
}

.hljs-constructor .hljs-string {
	color: #9ccc65!important;
}

.hljs-comment,
.hljs-quote {
	color: #b18eb1!important;
	font-style: italic!important;
}

.hljs-doctag,
.hljs-formula {
	color: #c678dd!important;
}

.hljs-deletion,
.hljs-name,
.hljs-section,
.hljs-selector-tag,
.hljs-subst {
	color: #e06c75!important;
}

.hljs-literal {
	color: #56b6c2!important;
}

.hljs-addition,
.hljs-attribute,
.hljs-meta-string,
.hljs-regexp,
.hljs-string {
	color: #98c379!important;
}

.hljs-built_in,
.hljs-class .hljs-title {
	color: #e6c07b!important;
}

.hljs-attr,
.hljs-number,
.hljs-selector-attr,
.hljs-selector-class,
.hljs-selector-pseudo,
.hljs-template-variable,
.hljs-type,
.hljs-variable {
	color: #d19a66!important;
}

.hljs-bullet,
.hljs-link,
.hljs-meta,
.hljs-selector-id,
.hljs-symbol,
.hljs-title {
	color: #61aeee!important;
}

.hljs-emphasis {
	font-style: italic!important;
}

.hljs-strong {
	font-weight: 700!important;
}

.hljs-link {
	text-decoration: underline!important;
}

/* Attempt at blink cursor */
.logo__cursor {
    display: inline-block;
    width: 15px;
    height: 1.5rem;
    background: #045FB4;
    margin-left: 5px;
    border-radius: 1px;
    -webkit-animation: cursor 1s infinite;
    animation: cursor 1s infinite;
}
@-webkit-keyframes cursor {
 0% {
  opacity:0;
 }
 50% {
  opacity:1;
 }
 to {
  opacity:0;
 }
}
@keyframes cursor {
 0% {
  opacity:0
 }
 50% {
  opacity:1
 }
 to {
  opacity:0
 }
}
```
*Note that I include the attribution to Riley Walz at the top, since I used his theme to get the home page to show up with titles and dates only.*

And here is the Custom JavaScript I use on this blog:
```js
/* Reading Time JS Widget */
const wpm = 200; // Average reading rate in words per minute (WPM)

let ps = document.querySelectorAll('p');
let wordCount = 0;
for (var i=0; i<ps.length; i++) {
	wordCount += ps[i].innerText.split(/\s+/).length;
}
let $time = document.querySelector('#post-body .dt-published');
if ($time) {
    const minuteToRead = Math.round(wordCount / wpm) > 0 ? Math.round(wordCount / wpm) : 1;
	$time.style.display = 'inline-block';
	$time.insertAdjacentHTML("afterend", '<span style="color: #73747b"> &middot; ' + minuteToRead + ' min read</span>');
}

/* Add blinking cursor to blog title */
const blogTitle = document.getElementById("blog-title");
const blogTitleChildNodes = blogTitle.childNodes;
blogTitleChildNodes[0].innerHTML += '<span class="logo__cursor"></span>';

/* Custom Footer*/
const customFooterHTML = `Copyright © 2018 - ${new Date().getFullYear()} by <a class="home pubd" href="https://dinobansigan.com/" target="_blank">Dino Bansigan</a><br />The opinions expressed herein are my own and do not represent those of my employer<br />or any other third-party views in any way.<br />This work is licensed under <a class="home pubd" href="https://creativecommons.org/licenses/by-nc-sa/4.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-NC-SA 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/sa.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1"></a><br />powered by <a class="home pubd" href="https://write.as/">write.as</a>`;
let x = document.querySelector('footer').getElementsByTagName('nav')[0];
x.innerHTML = customFooterHTML;
```