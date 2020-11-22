---
layout: post
title: HandyNotes Midsummer Festival Updated to Version 1.1
categories: [HandyNotes Summer Festival]
---

<script>const whTooltips = { colorLinks: false, iconizeLinks: false, renameLinks: false };</script>
<script src="https://wow.zamimg.com/widgets/power.js"></script>

After a two-month long break from World of Warcraft, I return bearing gifts!

Today's gift is a significant update to HandyNotes Midsummer Festival.  While end users will likely not notice any difference, a lot the addon's code has been changed in a similar way to a HandyNotes Lunar Festival update earlier this year.

Most notably, the addon now has an "automatic on/off switch" that makes use of the in-game calendar.  HandyNotes Midsummer Festival has gained sentience and is now able to detect when the event has started and will place marker icons on the worldmap and minimap without requiring players to log out or reload the user interface.  Similarly, the addon will also hide the icons automatically after the event has ended.

The way the addon handles bonfires you have already visited has also been overhauled.  Blizzard's `IsQuestFlaggedComplete()` API has proven to be unsuitable for our needs, so the addon now uses an internal table of completed quests that is updated every time a quest is completed.  This new method should fix marker icons remaining on the minimap after you visit a bonfire.

HandyNotes Midsummer Festival is currently available for download from [CurseForge](https://www.curseforge.com/wow/addons/handynotes_summerfestival) and requires [HandyNotes](https://www.curseforge.com/wow/addons/handynotes) to function.  If you want to report an error or request a new feature then please submit a support ticket on either Twitter or file a bug report on GitHub, WoWace, or Curse.  I read every message I receive and do my best to resolve problems as soon as possible.

The 2015 Summer Festival began yesterday and will end on July 5th.  Good luck!

Patch Notes:

* Flagged as up-to-date with Patch 6.1.
* Added an "automatic on/off switch" to enable/disable the addon when the Midsummer Fire Festival begins/ends.
* Added icons to show [Zidormi](https://www.wowhead.com/npc=63546/zidormi]'s location in Dustwallow Marsh and the Blasted Lands. Talk to her if you can't find the bonfires in those zones.
* Fixed bonfire markers remaining stuck on the minimap after visiting that bonfire.
* Fixed bonfire markers not showing on the worldmap due to terrain phasing.
* Fixed TomTom waypoints not working properly.
* Improved tooltip text slightly.
* Removed Cartographer support.