---
{"dg-publish":true,"permalink":"/snippets/webarchiver-cli/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# webarchiver CLI
Updated `07272022-091431`

- [newzealandpaul/webarchiver: Webarchiver allows you to create Safari .webarchive files from the command line. This project was featured on the Github blog in December 2008 👍](https://github.com/newzealandpaul/webarchiver)
- [webarchiver CLI](drafts://open?uuid=CAABBB06-186C-437D-BC30-65844BDBEC2B)
- [WTF](https://davidblue.wtf/drafts/CAABBB06-186C-437D-BC30-65844BDBEC2B.html)
- [Simplenote Local](simplenote://note/7e7592d5c20041c0a2ed8610e6c70e8e)
- [Simplenote Publish](http://simp.ly/publish/nyQqq5)
- [Things](things:///show?id=BjF5CaJMwPbPzgzkKrdt6q)

---

## Webarchiver allows you to create Safari .webarchive files from the command line. Webarchives are a convenient way to store a webpage and its associated files (images, css, javascript, etc) in a single file. It is very simple to use:

`./webarchiver -url https://www.google.com -output google.webarchive`

## Usage

```
$./webarchiver

webarchiver 0.9
Usage: webarchiver -url URL [-js JAVASCRIPT] -output FILE
Example: webarchiver -url https://www.google.com -output google.webarchive
-urlhttp:// or path to local file
-js Custom JavaScript to execute after loading the page
-output File to write the webarchive to.
```

Do not forget the ‘http://’ if you want to archive a webpage. If no
‘http://’ is present then webarchiver attempts to archive a local file.

## Download

The easiest way to install webarchiver is by using HomeBrew or MacPorts.
   
```
$ brew install webarchiver

$ sudo port install webarchiver
```

## Release notes

Version 0.10 : Added the ability to execute custom javascript on page load. Thanks [Viktor Szakats](https://github.com/vszakats)

Version 0.9 : Removed man page template. Updated Version number in code. Thanks [Kurt Hindenburg][]

Version 0.8 : [Matias Piipari][] fixed error codes.

Version 0.7 : 

- Modernized and improved the code.
- Support for loading local HTML files without an extension.
- If the output path is a folder, we now save the webarchive there.
- **Big thanks to [Jan Weiß][] for the work done in this release**

Version 0.6 : Cleaned up Github release.

Version 0.5 : More robust KBWebArchiver ([Keith Blount][] and [Jan Weiß][]).

Version 0.4 : Code maintenance and cleanup ([Jan Weiß][]).

Version 0.3 : Changed URL and sorted out source for git.

Version 0.2 : [John Winter][] fixed page loading issue.

Version 0.1 : Initial release.

## Credits
-   [Kurt Hindenburg][] for maintenance. 
-   [Matias Piipari][] for fixing error codes.
-   [Jan Weiß][] for his code fixes, clean up, 0.4 and 0.7 release. 
-   [Keith Blount][] for his very
useful KBWebArchiver class.
-   [John Winter][] for testing and bug fixing. Thanks John.
-   [Rob Griffiths][] for hosting a copy of the source when my blog was
down.
-   Boey Maun Suang for creating a MacPort
-   [Viktor Szakats](https://github.com/vszakats) for js option and HomeBrew.

  [Matias Piipari]: https://github.com/mz2
  [MacPorts]: https://www.macports.org/
  [Jan Weiß]: https://github.com/JanX2/webarchiver
  [John Winter]: http://www.shipsomecode.com/
  [Keith Blount]: https://www.literatureandlatte.com/
  [Rob Griffiths]: https://www.macosxhints.com/
  [Kurt Hindenburg]: https://github.com/kurthindenburg?tab=activity

---

webarchiver -url {url} -output webarchiver/{name}.webarchive

Tags:
  .webarchive, archive, macos, odette, snippets, web