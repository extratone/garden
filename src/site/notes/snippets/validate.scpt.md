---
{"dg-publish":true,"permalink":"/snippets/validate-scpt/","dgHomeLink":true,"dgPassFrontmatter":false}
---

validate.scpt
set the ClipURL to (the clipboard as string)
try
	set scriptCmd to "curl -I -L -s \"" & ClipURL & "\" | grep -c \"^HTTP/[^ ]* 200\""
	set scriptResult to do shell script scriptCmd
on error
	set scriptResult to ""
end try
if scriptResult is equal to "1" then
	return escapedURL(ClipURL)
else
	beep
	return "XX " & escapedURL (ClipURL)
end if

on escapedURL(theURL)
	set resultURL to ""
	repeat with eachChar in characters of theURL
		set eachCharNum to ASCII number of eachChar
		if eachCharNum = 37 then
			set resultURL to resultURL & "%%"
		else
			set resultURL to resultURL & eachChar
		end
	end
	return resultURL
end

Tags:
  applescript, snippets