---
{"dg-publish":true,"permalink":"/snippets/number-selectionby-tracks-scpt/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# NumberSelectionbyTracks.scpt

- [applescripts/Number Selection by Tracks.applescript at main · kotfu/applescripts](https://github.com/kotfu/applescripts/blob/main/src/Number%20Selection%20by%20Tracks.applescript)

---
(*
This script takes the selected tracks in iTunes, and incrementaly numbers them by
setting track metadata
*)
tell application "iTunes"
	set num to 1
	if selection is not {} then -- there ARE tracks selected...
		set mySelection to selection
		repeat with aTrack in mySelection
			#log (get name of aTrack)
			set (track number of aTrack) to num
			set num to num + 1
		end repeat
	end if
end tell

Tags:
  applescript, legacy, macos, snippets