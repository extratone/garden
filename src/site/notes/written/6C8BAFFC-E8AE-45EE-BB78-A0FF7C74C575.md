---
share: true
dg-publish: true
---
# Spy Kids 3 Spam (macOS) Shortcut Documentation

![Juni Warning](https://user-images.githubusercontent.com/43663476/149655618-67b3ac6a-50d6-4eb6-aeca-370eddef670f.png)

## Send one of cinema's great screenplays, line-by-line, to a recipient of your choice via imessage-ruby. 

- [**RoutineHub Page**](https://routinehub.co/shortcut/10873)
- [iCloud Share Link](https://www.icloud.com/shortcuts/be6f193dad2b4044b2b1cf165ff08c14)
- [iCloud Share Link(PRE-DOCS)](https://www.icloud.com/shortcuts/caf776e2ba7d481ea03492a7241db7bd)
- [imessage-ruby — Homebrew Formulae](https://formulae.brew.sh/formula/imessage-ruby)
- [ShareShortcuts](https://shareshortcuts.com/shortcuts/1606-spy-kids-3-spam-macos.html)

[[w:Birthday|w:Birthday]]
<video controls>
  <source src="https://user-images.githubusercontent.com/43663476/149640755-91ce7a1a-1c77-4148-aefe-9389eb115d16.mp4">
</video>

## Requirements
[**imessage-ruby**](https://formulae.brew.sh/formula/imessage-ruby)

`brew install imessage-ruby`

## About

It feels blasphemous to say so, but I believe I may have actually outdone the Original Masterpiece, [Bee Movie Spam](https://routinehub.co/shortcut/2623/)...

This shortcut uses a `Run Shell Script` action commanding [iMessage-ruby](https://formulae.brew.sh/formula/imessage-ruby) on macOS to send the entirety of [the *Spy Kids 3* screenplay](https://github.com/extratone/i/blob/main/assets/spykids3.md) (or at least... I think it's the actual screenplay - not actually sure, nor does it matter,) line-by-line to a specified phone number via Messages. 

![Spy Kids 3 Spam Source](https://user-images.githubusercontent.com/43663476/149641065-0e497ea9-89d5-470a-8932-8cd48bd65a07.png)

The command itself:

`imessage --text "Repeat Item" --contacts "Provided Input"`

By my count, the screenplay text totals 6937 words in 1559 lines, which means 1559 messages total. I've tested it once all the way through just to confirm the cycle will complete, but didn't think to set a timer. It was more than 10 minutes, less than 30, I'd say.

I left my own phone number - +15738234380 - in the `Default Number` field of the [Ask for Input](https://www.matthewcassinelli.com/actions/ask-for-input/) action very much on purpose - I promise it'll make my day if you use me as a test subject.

- [Video Demo](https://www.instagram.com/p/CYxP3HppgOi/)
- [Source Files](https://github.com/extratone/i/tree/main/shortcuts/Spy%20Kids%203%20Spam)