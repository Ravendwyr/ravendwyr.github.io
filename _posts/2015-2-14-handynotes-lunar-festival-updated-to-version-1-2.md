---
layout: post
title: HandyNotes Lunar Festival Updated to Version 1.2
categories: [HandyNotes Lunar Festival]
---

<script>const whTooltips = { colorLinks: false, iconizeLinks: false, renameLinks: false };</script>
<script src="https://wow.zamimg.com/widgets/power.js"></script>

The annual Lunar Festival will be starting once again, this time on February 16th rather than the usual early January.  In preparation of the event's arrival, a new version of HandyNotes Lunar Festival was made available this morning.

This is a fairly major update which includes an "automatic on/off switch" of sorts.  The addon is now able to detect when the event has started and will place marker icons on the worldmap and minimap without requiring the user to log out or reload the UI first.  Similarly, the addon will also hide the icons automatically after the event has ended.

The way the addon handles Elder NPCs you have already visited has also been overhauled.  Blizzard's `IsQuestFlaggedComplete()` API has proven to be unsuitable for our needs, so the addon now uses an internal table of completed quests that is updated every time a quest is completed.  This new method should fix marker icons remaining on the minimap after you visit an Elder.

These changes should make HandyNotes Lunar Festival better than ever before, however if you encounter any problems please don't hesitate to get in touch.

The new version of HandyNotes Lunar Festival is available to download from [CurseForge](https://www.curseforge.com/wow/addons/handynotes_lunarfestival) and requires [HandyNotes](https://www.curseforge.com/wow/addons/handynotes) to work.  Remember that the map pins will only appear while the Lunar Festival is active!

The 2015 Lunar Festival will start on February 16th and will end on March 2nd.  Good luck!

Patch Notes:

* Flagged as up-to-date with Patch 6.0.
* Added an "automatic on/off switch" to enable/disable the addon when the Lunar Festival begins/ends.
* Added an icon that shows [Zidormi](https://www.wowhead.com/npc=88206/zidormi)'s location in the Blasted Lands. Talk to her if you can't find [Elder Bellowrage](https://www.wowhead.com/npc=15563/elder-bellowrage).
* Fixed an unclickable menu entry for users who don’t have TomTom installed.
* Fixed icons remaining stuck on the minimap.
* Removed Cartographer support as the addon has been dead for years.