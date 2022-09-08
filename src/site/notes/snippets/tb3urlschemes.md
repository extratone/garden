---
{"dg-publish":true,"permalink":"/snippets/tb3urlschemes/","dgHomeLink":true,"dgPassFrontmatter":false}
---

tb3urlschemes

---
created: 2021-04-07T02:37:11Z
folder: Gist
gist: https://gist.github.com/87eadaf96d13b7bef8eaa2565414d257
language: Markdown
modified: 2021-04-07T02:38:16Z
notes: |
    A list of supported URL schemes in Tweetbot 3 for MacOS.
    Author: extratone (https://gist.github.com/87eadaf96d13b7bef8eaa2565414d257)
title: tb3urlschemes.md
---

# Supported Tweetbot 3 URL Schemes
Via [_MacStories_ reference](https://tapbots.net/tweetbot3/support/url-schemes/) for their original review.
```
tweetbot://<screenname>/timeline
tweetbot://<screenname>/mentions
tweetbot://<screenname>/retweets
tweetbot://<screenname>/direct_messages
tweetbot://<screenname>/lists
tweetbot://<screenname>/favorites
tweetbot://<screenname>/search
tweetbot://<screenname>/search?query=<text>
tweetbot://<screenname>/status/<tweet_id>
tweetbot://<screenname>/user_profile/<profile_screenname>
tweetbot://<screenname>/post
tweetbot://<screenname>/post?text=<text>
tweetbot://<screenname>/post?text=<text>&callback_url=<url>&in_reply_to_status_id=<tweet_id>
tweetbot://<screenname>/search?query=<text>&callback_url=<url>
tweetbot://<screenname>/status/<tweet_id>?callback_url=<url>
tweetbot://<screenname>/user_profile/<screenname|user_id>?callback_url=<url>
tweetbot://<screenname>/follow/<screenname|user_id>
tweetbot://<screenname>/unfollow/<screenname|user_id>
tweetbot://<screenname>/favorite/<tweet_id>
tweetbot://<screenname>/unfavorite/<tweet_id>
tweetbot://<screenname>/retweet/<tweet_id>
tweetbot://<screenname>/list/<list_id>?callback_url=<url>
```
The argument callback_url is an URL encoded URL that will be opened in Safari once the Post view closes.