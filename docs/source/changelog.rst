Changes in ThinkUp
==================

Beta 0.12 - 13 May 2011
-----------------------

**New:**

* User invitation system: If registration is closed to the public, an admin can generate a user invitation link good for one user registration
* Update available notifications when there's a new version of ThinkUp available (admins only)
* Application setting to disable JSON API access (admins only)
* Application setting to set default service user to display when visiting ThinkUp, rather than always showing the last updated user (admin-only)
* Full support for servers running https://
* Improved interface for switching service user, running the crawler, and reorganized the settings tabs to make it easier/clearer what does what
* Added links to help documentation throughout the application

**Fixed:**

* Invalid JSON returned by the Post API
* SlickGrid export button no longer opens a new tab
* Doesn't show follower count milestones unless they're within 10 days, weeks, or months (i.e., no more "You will reach 1,000 followers in 954 weeks")
* Deprecated the Embed Thread plugin and made it core functionality, with the option to disable it in Settings > Application
* Multiple embedded ThinkUp threads on a given web page no longer overwrite each other; Added permalinks to embedded threads
* Removed Twitter plugin former friends/followers and not mutual data listings (which didn't work anyway)

**IMPORTANT BACKWARD-COMPATIBILITY NOTICE**

Beta 12 will break any embedded ThinkUp threads from earlier versions. Please update any embed code you've published
on the web from earlier versions of ThinkUp.

Beta 0.11 - 25 April 2011
-------------------------

**Bugfix Release**

Beta 11 is a **REQUIRED UPDATE** for all installations of ThinkUp prior to April 25.

* Fixes a potential information vulnerability in older versions of ThinkUp that could reveal private posts that are stored by the application.
* Fixes a PHP Notice on ThinkUp API calls in some server environments and updates API documentation.
* Adds Security and Data Privacy documentation.
* Fixes bug where Dashboard menu links are incorrect after logout.


Beta 0.10 - 20 April 2011
-------------------------
**New:**

* Dashboard, post, and user page redesign: Lefthand menu has a new active tab style; users include links to both their profile on the originating service (i.e., Twitter.com) and internal ThinkUp page. The user page is now in the app-wide ThinkUp template.
* Post API: ThinkUp's posts, replies, and retweets are now available in a JSON-based API. See the complete :doc:`complete Post API documentation </userguide/api/index>`.
* Top 20 words redesign: On a given post's page, the top 20 most-frequently mentioned words display by default (you no longer have to click on "Top 20 words" in the menu, which has been removed). The Top 20 words have been redesigned to be more "tappable."
* Twitter Web Intents: Easily reply, retweet, or favorite any tweet you see in ThinkUp, directly from ThinkUp's interface. More info: http://expertlabs.org/2011/04/twitters-web-intents.html
* Sticky dashboard navigation: On multi-account installations, when viewing an individual post, clicking on the Dashboard link you will return you to the current instance (not the most recently updated instance).
* Application documentation: Launched official application documentation which developers will submit along with each patch to the project. Eventually these docs will be hosted on thinkupapp.com, but the initial version is available at http://readthedocs.org/docs/thinkup/en/latest/. Background information: http://groups.google.com/group/thinkupapp/browse_thread/thread/aee02b16d968c8ed/656b0849117acd0b
* (Developers) Error-level only logging: New config file value, ``$THINKUP_CFG['log_verbosity']``, lets you set the log to only log errors.

**Fixed:**

* Broken link in ThinkUp user activation email.
* Inaccurate rendering of the Broadcaster/Conversationalist bar chart on the Dashboard.
* Favorites search via SlickGrid.
* Google Map display of post replies and retweets: Replies and retweets are no longer cut off on the page.
* SlickGrid's export button: This mostly works; but it's still an open issue which needs a better solution. You can export posts from SlickGrid's search results. Currently it opens a new tab; we're working on making it work within the current tab/window.
* Missing Zip library error message in Backup controller: The Backup controller now gracefully handles a server setup without the Zip library installed.
* Follows table indexes optimized for faster retrieval.
* CrawlerLockedException on a server with multiple installs but different mutexes: Multiple crawls can now run side-by-side on a server with multiple installations if they talk to different databases.
* Fixed "No plugin object defined" error when deactivating a plugin.
* SlickGrid search results for Facebook; also added permalinks to both Twitter.com and inside ThinkUp to SlickGrid Twitter results.
* Several potential security issues in ThinkUp's WordPress plugin: Download the latest version at https://github.com/downloads/ginatrapani/ThinkUp/thinkup_for_wordpress_0.8.zip
* Renamed Windows-hostile filenames.
* Developers: Fixed several test failures; upgraded the testing framework to SimpleTest 1.1 alpha, which lets developers turn on E_STRICT error level reporting for bulletproof coding and testing.
* Developers: More tests are now using the FixtureBuilder library instead of raw SQL inserts.

**TODO: Port changelogs from pre-beta 10 releases into the text of this page**

Beta 0.9 - 17 Mar 2011
----------------------
http://groups.google.com/group/thinkupapp/browse_thread/thread/71a3bc3c8f9f14f?hl=en_US

Beta 0.8 - 28 Jan 2011
-----------------------
http://groups.google.com/group/thinkupapp/browse_thread/thread/6931355e49a546f5
 
Beta 0.7 - 27 Dec 2010
----------------------
http://groups.google.com/group/thinkupapp/browse_thread/thread/62a4cc4d6b948ff1


Beta 0.6 - 13 Dec 2010
----------------------
https://groups.google.com/forum/#topic/thinkupapp/DxuKJmAdB-c
 
Beta 0.5 - 22 Nov 2010
----------------------
http://groups.google.com/group/thinkupapp/browse_thread/thread/4a55784c0b758a3a
 
Beta 0.4 - 14 Nov 2010
----------------------
http://groups.google.com/group/thinkupapp/browse_thread/thread/606567695212e687
 
Beta 0.3 - 19 Oct 2010
----------------------
http://groups.google.com/group/thinkupapp/browse_thread/thread/fb54106f4d4bdba9

Beta 0.2 - 4 Oct 2010
---------------------
http://groups.google.com/group/thinkupapp/browse_thread/thread/b384ccfce40ff7fc

Beta 0.1 - 27 Sept 2010
-----------------------
http://groups.google.com/group/thinkupapp/browse_thread/thread/879316197e4aeb7a/17d32d0a80712dc8

