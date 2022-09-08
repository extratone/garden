---
{"dg-publish":true,"permalink":"/snippets/openin-marked2-scpt/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# OpeninMarked2.scpt

- [marked-bonus-pack/OpenInMarked.applescript at main · kotfu/marked-bonus-pack](https://github.com/kotfu/marked-bonus-pack/blob/main/AppleScript/OpenInMarked.applescript)

---
-- Open in Marked 2
-- Attempts to open the currently-edited document in Marked 2 for previewing
-- Based on ideas by Lri <https://gist.github.com/1077745>
-- with contributions from Donald Curtis <https://github.com/milkypostman>

---NV/nvALT configuation---------------------------------------------------
-- * Set NV/nvALT to store text files to disk
-- * Enter the full UNIX/POSIX path to your notes folder in nvNoteFolder
-- * Enter your default file extension (.txt,.md,etc.) in nvNoteExtension
-- It won't always work, but it will try. It's a temporary hack; 
-- nvALT will soon have an AppleScript command to access the file directly.
property nvNoteFolder : "/Users/username/pathtonotes/" -- include trailing slash
property nvNoteExtension : ".md" -- include leading dot
---------------------------------------------------------------------------on run {}
tell application "System Events"
	set frontApp to (name of first process whose frontmost is true)
end tell

set f to false
set flist to {}

--Marked 2 (if Marked 2 is foreground, hide Marked 2 and end script)
if frontApp is "Marked 2" then
	tell application "System Events" to set visible of process "Marked 2" to false
	return
	--Notational Velocity/nvALT
else if (frontApp is "Notational Velocity") or (frontApp is "nvALT") then
	try
		tell application "System Events" to tell process frontApp
			-- Grab the text in the search field, hopefully this will be the filename
			set p to value of text field 1 of group 1 of toolbar 1 of window 1
			try -- look for it in nvNoteFolder with the nvNoteExtension suffix
				set f to POSIX file (nvNoteFolder 

Tags:
  applescript, macos, marked2, md, snippets