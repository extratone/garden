---
{"dg-publish":true,"permalink":"/snippets/telegram-android-attheme-2/","dgHomeLink":true,"dgPassFrontmatter":false}
---

telegram-android-attheme-2

---
created: 2021-09-20T13:18:35Z
folder: Gist
gist: https://gist.github.com/e8cbe5b4fb7820ad9505eea905465e47
language: Markdown
modified: 2021-09-20T13:18:38Z
notes: |
    Comprehensive reference description of telegram theming elements
    Author: extratone (https://gist.github.com/e8cbe5b4fb7820ad9505eea905465e47)
title: Telegram Theming Reference.md
---

| Key                                               | Description                                                  |
| ------------------------------------------------- | ------------------------------------------------------------ |
| _Generic_                                         |                                                              |
| windowBackgroundWhite                             | Main background colour                                       |
| windowBackgroundWhiteGrayText2                    | Subtitle text for text items with descriptors (mobile, username etc.) |
| windowBackgroundWhiteBlueHeader                   | Title of settings menu items (\*)                            |
| windowBackgroundWhiteBlueText4                    | “Change chat background” text/icon                           |
| divider                                           | Dividing line between clickable items                        |
| listSelectorSDK21                                 | Ripple overlay when pressing list/menu item (dimmed)         |
| chats_action[Icon/Background/PressedBackground]   | [Icon/background/background when tapped] of floating action button (FAB) in chat/calls list screen |
| featuredStickers_addButton                        | /!\ Also affects phone icon in calls list screen             |
| actionBarDefaultSelector                          | /!\ Unknown /!\                                              |
| actionBarDefault                                  | Background of header bar                                     |
| actionBarDefaultIcon                              | Icons in header bar (hamburger/search/ellipse/etc.)          |
| actionBarDefaultTitle                             | Main text in header bar                                      |
| actionBarDefaultSubtitle                          | Last seen time text in header bar                            |
| actionBarDefaultSearch                            | Text typed into the searchbar                                |
| actionBarDefaultSearchPlaceholder                 | “Search” text before typing in the (inchat) searchbar        |
| actionBarActionModeDefaultIcon                    | Header bar background when selecting messages                |
| actionBarActionModeDefaultTop                     | OS statusbar when selecting messages                         |
| actionBarActionModeDefaultSelector                |                                                              |
| actionBarDefaultSubmenuBackground                 | Background of ellipsis/dropdown menu                         |
| actionBarDefaultSubmenuItem                       | Text of ellipsis/dropdown menu items                         |
| actionBarDefaultSubmenuItemIcon                   | Icons of ellipsis/dropdown menu items                        |
| player_progressBackground                         | Dimmed darker line of all progress bars/sliders in settings  |
| player_progress                                   | Foreground/dot of all progress bars/sliders in settings      |
| switchTrack                                       | Toggle switch icon when disabled - also hue of 2/3 line preview in settings |
| switchTrackChecked                                | Toggle switch icon when enabled                              |
| chats_callRecieved[Red/Green]Icon                 | Arrow in calls screen of [failed/successful] calls           |
|                                                   |                                                              |
| _Chats List_                                      |                                                              |
| profile_tabSelected[Line/Text]                    | See entry in #User Profile (may be a bug?)                   |
| profile_tabText                                   | See entry in #User Profile (may be a bug?)                   |
| avatar_text                                       | User initials of placeholder avatar for contact with no profile pic |
| avatar_background[Colour]                         | Background of placeholder avatar for contact with no profile pic |
| key_graySectionText                               | /!\ Month name in “Saved Messages” file lists - may be elsewhere too |
| graySection                                       | Dark between cards in “Saved Messages”/“New Message” dialogue |
| chats_menuBackground                              | Background of sidebar menu                                   |
| chats_menuName                                    | Username in sidebar menu (also day/night toggle)             |
| chats_menuPhone                                   | Phone number in sidebar menu                                 |
| chats_menuPhoneCats                               | same as chats_menuPhone, sometimes?                          |
| chat_serviceBackground                            | Background of forward button, internal link to group, etc    |
| chat_service[Text/Link/Icon]                      | [Text/Link/Icon] of forward button, internal link to group, etc |
| chats_menuTopShadow                               | /!\ Unknown /!\                                              |
| chats_menuTopShadowCats                           | Bottom “shadow” for section of sidebar menu containing username |
| chats_menuTopBackgroundCats                       | /!\ Unknown /!\                                              |
| chats_menuTopBackground                           | Background for section of sidebar menu containing username   |
| chats_menuItemIcon                                | Icons for elements in sidebar menu                           |
| chats_menuItemText                                | Text for elements in sidebar menu                            |
| chats_archiveText                                 | /!\ Unknown /!\                                              |
| inappPlayerBackground                             | Background of mini music player                              |
| inappPlayerPlayPause                              | Play/pause icon of mini music player                         |
| inappPlayerTitle                                  | Track title of mini music player                             |
| inappPlayerPerformer                              | Artist of mini music player                                  |
| inappPlayerClose                                  | Close (x) icon of mini music player                          |
| checkbox                                          | background of “selected” chat tickmark icon                  |
|                                                   |                                                              |
| _In Chat_                                         |                                                              |
| chat_status                                       | “Online” status below contact name in top bar                |
| chat_muteIcon                                     | “Muted” icon by recipient name                               |
| chat_lockIcon                                     | Secret chat padlock icon                                     |
| avatar_nameInMessage[Colour]                      | User's name in message bubble (groups)                       |
| chat_inBubble                                     | Inbound message bubble background                            |
| chat_inBubbleSelected                             | Inbound message bubble background, when selecting multiple messages |
| chat_inBubbleShadow                               | /!\ Unknown /!\                                              |
| chat_outBubbleShadow                              | /!\ Unknown /!\                                              |
| chat_outBubble                                    | Outbound message bubble background                           |
| chat_outBubbleGradient                            | Background vertical gradient across all bubbles, set alpha to 0 to disable |
| chat_outBubbleSelected                            | Outbound message bubble background, when selecting multiple messages |
| chat_outBubbleGradientSelectedOverlay             | /!\ Unknown /!\                                              |
| chat_serviceText                                  | /!\ Unknown /!\ - appears defunct                            |
| chat_serviceLink                                  | /!\ Unknown /!\ - appears defunct                            |
| chat_serviceIcon                                  | /!\ Unknown /!\ - appears defunct                            |
| chat_serviceBackground                            | Message selected left hand tickbox (dimmed for some reason?) |
| chat_serviceBackgroundSelected                    | /!\ Unknown /!\                                              |
| chat_messageTextIn                                | Inbound message bubble text                                  |
| chat_messageTextOut                               | Outbound message bubble text                                 |
| chat_messageLinkIn                                | Inbound message bubble clickable link text                   |
| chat_messageLinkOut                               | Outbound message bubble clickable link text                  |
| chat_mediaTimeText                                | Sent timestamp on media messages (images etc.)               |
| chat_outSentCheck                                 | Outbound message sent tickmark                               |
| chat_outSentCheckSelected                         | Outbound message sent tick when selected                     |
| chat_outSentCheckRead                             | Outbound message read double tick                            |
| chat_outSentCheckReadSelected                     | Outbound message read double tick when selected              |
| chat_outSentClock                                 | Outbound message sending clock icon                          |
| chat_outSentClockSelected                         | Outbound message sending clock icon when selected            |
| chat_inSentClock                                  | Inbound message sending clock icon                           |
| chat_inSentClockSelected                          | Inbound message sending clock icon when selected             |
| chat_mediaSentCheck                               | Outbound image sent tickmark                                 |
| chat_mediaSentClock                               | Outbound image sending clock icon                            |
| chat_[in/out]Views[Selected]                      | Views (eye) icon on message bubble in group chats [when message selected] |
| chat_mediaViews                                   | Views (eye) icon on images in group chats                    |
| chat_[in/out]Menu[Selected]                       | Unticked radio button on media (file/poll/etc.) [when message selected] |
| chat_mediaMenu                                    | /!\ Unknown /!\                                              |
| chat_[in/out]Instant                              | Lightning icon in [inbound/outbound] instant article links   |
| chat_[in/out]InstantSelected                      | /!\ Unknown /!\                                              |
| chat_[in/out]PreviewInstantText                   | “Instant View” text + outline in [inbound/outbound] instant article links |
| chat_[in/out]PreviewInstantSelectedText           | /!\ Unknown /!\                                              |
| chat_selectedBackground                           | Background behind selected message bubbles                   |
|                                                   |                                                              |
| chat_[in/out]ReplyLine                            | Line to the left of quoted text in [inbound/outbound] reply messages |
| chat_[in/out]ReplyNameText                        | Name of sender of message replied to in [inbound/outbound] messages |
| chat_[in/out]ReplyMessageText                     | Contents of message replied to in [inbound/outbound] messages |
| chat_[in/out]AudioSeekbar[Selected]               | Dimmed darker line of [inbound/outbound] music progress bar [when message selected] |
| chat_[in/out]AudioSeekbarFill[Selected]           | Foreground/dot of [inbound/outbound] music progress bar [when message selected] |
|                                                   |                                                              |
| _User Profile_                                    |                                                              |
| profile_tabSelected[Line/Text]                    | [Text/Line below] media type active tab - also in chats list when multiple chats selected |
| profile_tabText                                   | Name of media type inactive tab - also in chats list when multiple chats selected |
| profile_action[Icon/Background/PressedBackground] | [Icon/background/background when tapped] of FAB in profile/setttings screen |
|                                                   |                                                              |