---
{"dg-publish":true,"permalink":"/snippets/gather-cli/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# gather-cli
Updated `09042022-053114`

- [Source](https://brettterpstra.com/projects/gather-cli/)
- [Drafts](drafts://open?uuid=CAABBB06-186C-437D-BC30-65844BDBEC2B)
- [WTF](https://davidblue.wtf/drafts/CAABBB06-186C-437D-BC30-65844BDBEC2B.html)
- Simplenote Local
- Simplenote Publish

---

USAGE: gather [<options>] [<url>]

ARGUMENTS:
  <url>                   The URL to parse

OPTIONS:
  -c, --copy              Copy output to clipboard
  --env <env>             Get input from and environment variable
  -f, --file <file>       Save output to file path. Accepts %date, %slugdate, %title, and %slug
  --html                  Expect raw HTML instead of a URL
  --include-source/--no-include-source
                          Include source link to original URL (default: true)
  --include-title/--no-include-title
                          Include page title as h1 (default: true)
  --inline-links          Use inline links
  --metadata              Include page title, date, source url as MultiMarkdown metadata
  -p, --paste             Get input from clipboard
  --paragraph-links/--no-paragraph-links
                          Insert link references after each paragraph (default: true)
  --readability/--no-readability
                          Use readability (default: true)
  -s, --stdin             Get input from STDIN
  -t, --title-only        Output only page title
  --unicode/--no-unicode  Use Unicode characters instead of ascii replacements (default: true)
  --accepted-only         Only save accepted answer from StackExchange question pages
  --include-comments      Include comments on StackExchange question pages
  --min-upvotes <min-upvotes>
                          Only save answers from StackExchange page with minimum number of upvotes (default: 0)
  --nv-url                Output as an Notational Velocity/nvALT URL
  --nv-add                Add output to Notational Velocity/nvALT immediately
  --nvu-url               Output as an nvUltra URL
  --nvu-add               Add output to nvUltra immediately
  --nvu-notebook <nvu-notebook>
                          Specify an nvUltra notebook for the 'make' URL
  --url-template <url-template>
                          Create a URL scheme from a template using %title, %text, %notebook, %source, %date, %filename, and %slug
  --fallback-title <fallback-title>
                          Fallback title to use if no title is found, accepts %date
  --url-open              Open URL created from template
  -v, --version           Display current version number
  -h, --help              Show help information.

Tags:
  documentation, macos, odette, reference, scrape, simplenote, snippets