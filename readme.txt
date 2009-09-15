=== Twitter Digest  ===
Tags: twitter, tweet, post digest
Contributors: tbeck
Requires at least: 2.7
Tested up to: 2.8.4
Stable Tag: 1.8.3

Creates a daily post containing tweets from a twitter account. 

== Description ==

This plugin uses the pseudo-cron facility available in Wordpress to publish a
daily post of tweets from the previous day.  It is based on Alex King's Twitter Tools plugin
found at http://alexking.org/projects/wordpress.

Notes:

- This plugin has not been tested on anything other than Wordpress 2.7 and
above  (If anyone wants to try an old version, let me know.)
- I used code and knowledge garnered from Alex King's Twitter Tools to build
this plugin.  See http://alexking.org/projects/wordpress
- A maximum of 20 tweets will be shown per post (due to Twitter API
limitation) and there will only be one post per day.  This means if you tweet
more than 20 times per day, not all the tweets will be shown. This may change
in the future.

== Installation ==

1. Download the plugin archive and expand it (you've likely already done this).
2. Put the 'twitter-digest.php' file into your wp-content/plugins/ directory.
3. Go to the Plugins page in your WordPress Administration area and click 'Activate' for Twitter Digest.
4. Go to the Twitter Digest Options page (Options > Twitter Digest) to set your Twitter account information and preferences.


== Configuration ==

There are a number of configuration options for Twitter Digest. You can find these in Options > Twitter Digest.

== ChangeLog ==

v1.8.3

- Fixed timezone issues
- Added button to reset plugin database

v1.8.2

- Fixed bug that caused HTML entities to be broken links
- Fixed issue with publishing in timezone that is not the same as the server timezone

v1.8.1

- Fixed bug that caused broken status link if @ message was not in reply to
  another message.

v1.8

- Added check for username/password on installation
- Added ability to ping the service from the options page.
- Added ability to specify the time of day the tweet post will be published

v1.7.2

- Added support for custom title

v1.7.1

- Fixed possible race condition issue
- Tweaked code layout
- Made min tweets always be at least 1
- Fixed bug with url in brackets not being made clickable.
- Fixed bug with 'in reply to' links not working 

v1.7

- Fixed bug that caused badness if minimum tweets was set to 0
- Added option to reverse the order of tweet display

v1.5

- Fixed bug with min tweets restriction
- Fixed bug with hashtag linkification

v1.4

- Fixed bug showing options error

v1.3

- Added options page
- Added minimum tweets required to post
- Fixed @twitter detection

v1.2

- Added ability to ignore @replies

v1.1

- Tweaked posting procedure so the post goes from the draft state to
published state, in order to trigger any hooks that would get triggered on a
'normal' post.
- Cleaned up post output

   
v1.0
- Basic tweet polling and posting.

== Contact ==

If you have questions or comments, please visit http://whalespine.org.

Thanks
Tim Beck
