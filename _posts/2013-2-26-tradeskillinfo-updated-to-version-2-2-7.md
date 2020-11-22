---
layout: post
title: TradeSkillInfo Updated to Version 2.2.7
categories: [TradeSkillInfo]
---

<script>const whTooltips = { colorLinks: false, iconizeLinks: false, renameLinks: false };</script>
<script src="https://wow.zamimg.com/widgets/power.js"></script>

Version 2.2.7 of TradeSkillInfo was released a few days ago with numerous updates to the recipe database and a small fix for the search feature in the Browser module.

This version is mostly a maintenance release and does not yet have the new Blacksmithing recipes in the database.  The information will be added in Version 2.2.8, which is currently scheduled for release shortly after World of Warcraft is updated to Patch 5.2 in a few weeks time.

There have also been a few confirmed cases of TradeSkillInfo causing "taint" issues recently, particularly with the new Grid-style raid frames.  They seem to be caused by the way TradeSkillInfo adds recipe information to item tooltips (recipe known by, learnable by, etc.) but, thankfully, doesn't seem to happen very often.  The entire tooltip support code will be completely re-written after the release of Version 2.2.8 and will hopefully solve this problem.

Patch Notes:

* Added more than 75 missing recipes that were added to World of Warcraft back in Patch 4.3.
* Fixed the recipes for [Exotic Leather](https://www.wowhead.com/spell=124627/exotic-leather), [Potion of Luck](https://www.wowhead.com/spell=114779/potion-of-luck), [Abyssal Shatter](https://www.wowhead.com/spell=69412/abyssal-shatter), [Maelstrom Shatter](https://www.wowhead.com/spell=104698/maelstrom-shatter), and [Imperial Silk](https://www.wowhead.com/spell=130325/song-of-harmony).
* Fixed a bug in the Browser module caused by trailing whitespace in the search box.
* Removed all support for [Runeforging](https://www.wowhead.com/spell=53428/runeforging).
* Removed some more useless code.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/tradeskill-info) or from [WoWInterface](https://www.wowinterface.com/downloads/info5473-TradeskillInfo.html).