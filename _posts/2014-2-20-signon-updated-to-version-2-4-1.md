---
layout: post
title: SignOn Updated to Version 2.4.1
categories: [SignOn]
---

SignOn has had a long overdue update this morning, bringing it back up to date and fixing a serious bug caused by the arrival of Patch 5.4.7.

SignOn uses "hyperlinks" embedded in the logon/logoff messages to obtain a player's name, which is then used to obtain additional character data such as class, level and notes.  Patch 5.4.7 changed the way these hyperlinks are constructed and this caused SignOn to be rendered useless.  Thankfully there were no Lua error messages caused by the changes, so SignOn could remain installed and enabled without causing any harm to anything.

Another "bug" that has been reported to me is a guild member appearing to log out twice without logging back in, like in the example above.  What actually happens is the character in question disconnected from the servers due to high latency or force-quitting the game instead of logging out the normal way.  Unfortunately this is a bug in World of Warcraft's code, not SignOn's.

Version 2.4.1 is strictly a maintenance build to fix problems caused by Patch 5.4.7.  There have been requests from the community to add a feature to strip the realm name out of the message as well as suppressing the duplicate logoff message.  These have not been forgotten or ignored, and will be added in future versions of SignOn.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/sign-on) or from [WoWInterface](https://www.wowinterface.com/downloads/info11801-SignOn.html).  Please do not hesitate to get in touch if you want to send any feedback.

Patch Notes:

* Fixed a bug caused by changes made in WoW Patch 5.4.7 which caused SignOn to stop functioning.
* Fixed the addon showing up as "out of date" in the addons list.
* Removed tekKonfig libraries as they are no longer needed.