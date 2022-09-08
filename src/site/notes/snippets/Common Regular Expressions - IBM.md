---
{"dg-publish":true,"permalink":"/snippets/common-regular-expressions-ibm/","dgHomeLink":true,"dgPassFrontmatter":false}
---

Common Regular Expressions - IBM

Tags: regex, learn, data
---

Common regular expressions
Last Updated: 2022-02-18

Use regular expressions to match patterns of text in the log source file. You can scan messages for patterns of letters, numbers, or a combination of both. For example, you can create regular expressions that match source and destination IP addresses, ports, MAC addresses, and more.

The following codes show several common regular expressions:

`\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3} \d{1,5} (?:[0-9a-fA-F]{2}\:){5}[0-9a-fA-F]{2} (TCP|UDP|ICMP|GRE) \w{3}\s\d{2}\s\d{2}:\d{2}:\d{2} \s \t .*? `

The escape character, or "\", is used to denote a literal character. For example, "." character means "any single character" and matches A, B, 1, X, and so on. To match the "." characters, a literal match, you must use "\."

Table 1. Common regex expressions

| Type           | Expression                           |
|----------------|--------------------------------------|
| IP Address     | d{1,3}.d{1,3}.d{1,3}.d{1,3}          |
| MAC Address    | (?:[0-9a-fA-F]{2}:){5}[0-9a-fA-F]{2} |
| Port Number    | d{1,5}                               |
| Protocol       | (TCP|UDP|ICMP|GRE)                   |
| Device Time    | w{3}sd{2}sd{2}:d{2}:d{2}             |
| Whitespace     | s                                    |
| Tab            | t                                    |
| Match Anything | .*?                                  |


\s
Tab	\t
Match Anything	.*?
Tip: To ensure that you don't accidentally match another characters, escape any non-digit or non-alpha character.

Tags:
  snippets