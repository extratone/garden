---
{"dg-publish":true,"permalink":"/snippets/stephen-millard-s-hook-obsidian-sc/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# Stephen Millard's Hook ⇦ ⇨ Obsidian Script
[Automation Documentation: Hooking Automations with Obsidian](https://www.thoughtasylum.com/2022/05/30/automation-documentation-hooking-automations-with-obsidian/)

```
-- to use Obsidian's advanced URL script, type this at the command line
-- defaults write com.cogsciapps.hook integration.obsidian.URL.scheme obsidian-advanced-URI
-- https://hookproductivity.com/help/integration/using-hook-with-obsidian

set sysinfo to system info
set osver to system version of sysinfo

considering numeric strings
    set isBigSur to osver ≥ "10.16"
end considering

if not isBigSur then
    set myURL to "obsidian://hook-get-address"
    set myScript to "open '" & myURL & "'"
    do shell script myScript
    delay 0.4
    repeat 50 times -- poll clipboard for ~2.5 seconds
        try
            if (the clipboard) is not equal to "" then
                exit repeat
            end if
        end try
        delay 0.05
    end repeat
    return the clipboard
    
end if


set prefUrl to ""
try
    set prefUrl to (do shell script "defaults read com.cogsciapps.hook integration.obsidian.URL.scheme")
    
on error errMsg
end try

if prefUrl is not "" and prefUrl is not "obsidian-default" and prefUrl is not "hook-file" and prefUrl is not "obsidian-advanced-URI" then
    
    
    -- An invalid value for com.cogsciapps.hook integration.obsidian.URL.scheme  has been set. There, we present the following options and set the default here.
    
    set thePrefChoices to {"obsidian-default (obsidian://)", "obsidian-advanced-URI (obsidian://advanced-uri)", "hook-file (hook://file/)"}
    set thePrefChoice to choose from list thePrefChoices with prompt "Please select one of the following URL schemes with which to interact with Obsidian:" default items {"obsidian-default (obsidian://)"}
    if thePrefChoice is not false then
        set x to thePrefChoice as text
        set AppleScript's text item delimiters to {" "}
        set prefUrl to text item 1 of x
        do shell script "defaults write com.cogsciapps.hook integration.obsidian.URL.scheme  " & prefUrl
    else
        return
    end if
    
    
end if


if prefUrl is "obsidian-advanced-URI" then
    set urlKey to "advanceduri"
    
    set callbackURL to "hook://x-callback-url/setCurrentNode%3FurlKey%3D" & urlKey & "%26plusencoded%3Dyes"
    set callbackURLError to "hook://x-callback-url/setCurrentNodeError"
    
    
    set myURL to "obsidian://hook-get-advanced-uri?" & "x-error=" & callbackURLError & "&x-success=" & callbackURL
    
    set myScript to "open '" & myURL & "'"
    
    do shell script myScript
    
else
    if prefUrl is "" or prefUrl is "obsidian-default" then
        set urlKey to ""
    else
        set urlKey to "%26urlKey%3Dfile"
    end if

    -- @sylumer modification: works for unique file names only
    -- Will work when files are moved, but we'll resort to using the clipboard (like the pre-Big Sur approach)
    -- so we can modify the returned Markdown link to remove the folder path.
    -- Stop doing this>>
    --set callbackURL to "hook://x-callback-url/setCurrentNode%3FtitleKey%3Dname" & urlKey
    --set callbackURLError to "hook://x-callback-url/setCurrentNodeError"
    --set myURL to "obsidian://hook-get-address?" & "&x-error=" & callbackURLError & "&x-success=" & callbackURL
    --set myScript to "open '" & myURL & "'"
    --do shell script myscript

    -- Start doing this>>
    do shell script "open 'obsidian://hook-get-address'"
    delay 0.1
    set oldDelims to my text item delimiters
    set my text item delimiters to "&file="
    set newLink to (first text item of (the clipboard)) & "&file="
    set newLinkTemp to (last text item of (the clipboard))
    set my text item delimiters to "%2F"
    set newLink to newLink & last text item of newLinkTemp
    set my text item delimiters to oldDelims
    return newLink
end if

-- Don't bother with this>>
--return "hook://x-callback-url/setCurrentNode"
```

Tags:
  macos, obsidian, snippets