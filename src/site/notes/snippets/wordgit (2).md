---
{"dg-publish":true,"permalink":"/snippets/wordgit-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

wordgit (2)

---
created: 2020-12-04T04:44:15Z
folder: Gist
gist: https://gist.github.com/72ad6ae736ae871fb3026bf73f229750
language: Markdown
modified: 2021-05-07T22:21:23Z
notes: |
    How to enable Git to read changes in .docx files so you can track revisions in Word... via Git!
    Author: extratone (https://gist.github.com/72ad6ae736ae871fb3026bf73f229750)
title: wordgit.md
---

# See diffs of .docx files with git `wdiff file.docx`. ([Source](https://github.com/vigente/gerardus/wiki/Integrate-git-diffs-with-word-docx-files))
====================================================

This section was inspired by Martin Fenner's ["Using Microsoft Word with git"](http://blog.martinfenner.org/2014/08/25/using-microsoft-word-with-git/).

To configure git diff:

1. [**Install pandoc**](http://pandoc.org/installing.html).

1. Tell git how to handle diffs of .docx files.
    1. Create or edit file ~/.gitconfig (linux, Mac) or "c:\Documents and Settings\user\.gitconfig" (Windows) to add

            [diff "pandoc"]
              textconv=pandoc --to=markdown
              prompt = false
            [alias]
              wdiff = diff --word-diff=color --unified=1

    1. In your paper directory, create or edit file .gitattributes (linux, Windows and Mac) to add

            *.docx diff=pandoc

    1.  You can commit .gitattributes so that it stays with your paper for use in other computers, but you'll need to edit ~/.gitconfig in every new computer you want to use.

Now you can see a pretty coloured diff with the changes you have made to your .docx file since the last commit

    git wdiff file.docx

To see all changes over time

    git log -p --word-diff=color file.docx

Track changes in Word (.docx) documents getting a diff with the commit.
=======================================================================

Automatically when running `git commit`.
----------------------------------------

This is only going to work from linux/Mac or Windows running git from a bash shell.

1. [**Install pandoc**](http://pandoc.org/installing.html). Pandoc is a program to convert between different file formats. It's going to allow us to convert Word files (.docx) to Markdown (.md).

1. **Set up git hooks to enable automatic generation and tracking of Markdown copies of .docx files.** 

    Copy these hook files to your git project's `.git/hooks` directory and rename them, or soft-link to them with `ln -s`, and make them executable (`chmod u+x *.sh`):

    * [pre-commit-git-diff-docx.sh](https://github.com/vigente/gerardus/blob/master/shell-script/pre-commit-git-diff-docx.sh) -> .git/hooks/pre-commit
    * [post-commit-git-diff-docx.sh](https://github.com/vigente/gerardus/blob/master/shell-script/post-commit-git-diff-docx.sh) -> .git/hooks/post-commit

    Now every time you run `git commit`, the pre-commit hook will automatically run before you see the window to enter the log message. The hook is a script that makes a copy in Markdown format (.md) of every .docx file you are committing. The post-commit hook then amends the commit adding the .md files.

Manually by creating a Markdown copy of the .docx file.
-------------------------------------------------------

This works in linux, Mac and Windows.

1. [**Install pandoc**](http://pandoc.org/installing.html).

1. **Edit your Word document** as needed.

1. **Run pandoc** from the linux or Windows command line. This will create a Markdown version of your file (without Figures, but with equations in latex format)

        pandoc -s file.docx -t markdown -o file.md

1. **Update the ChangeLog**

1. **Commit both files with git**

        git add file.docx file.md
        git commit