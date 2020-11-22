---
layout: post
title: TradeSkillInfo Updated to Version 2.3.10
categories: [TradeSkillInfo]
---

The Legion expansion pre-patch is upon us and as usual with a massive update such as this a whole load of addons will need a whole load of updates.

It has been a very long time since the last news article about a TradeSkillInfo update (despite the amount of updates the addon has received since then) and today's post marks the first working version for Patch 7.0.3.

There has been quite a large number of changes with the Legion pre-patch.  The professions UI has been completely redesigned into a "double-wide" window for easier navigation and now has "Learned" and "Unlearned" tabs that show all of the available recipes in the game as well as an idea where to find them.  This change does make some features in the Browser module somewhat redundant however.  Action will be taken in the future to discern which features can be ported to use Blizzard's new API or which ones could be pruned altogether.

Unfortunately not everything is good news. The skill level and profit margin labels have been disabled on the professions UI for the time being.  This is a temporary change while I figure out the best way to make it work with the new window and the info is still available on the Browser module.

The datamining script used to gather recipe information also received some love.  The script now only retrieves information from WoWhead instead of GetBuffed as their database has proven to be unusable as of late especially with the Legion pre-patch.  A huge thanks goes to WoWhead and the staff who allow me to abuse their website like this.  I will be making more tweaks over time to speed up and streamline the mining.

You can download this new version of TradeSkillInfo from [CurseForge](https://www.curseforge.com/wow/addons/tradeskill-info) or from [WoWInterface](https://www.wowinterface.com/downloads/info5473-TradeskillInfo.html).  As always, if you find any problems feel free to get in touch.

See you on the Broken Isles!

Patch Notes:

* Marked as up-to-date with Patch 7.0.3.
* Updated the dataminer to only retrieve information from WoWhead instead of GetBuffed.
* Updated the recipe database.
* Fixed a bunch of startup errors caused by changes in the API.
* Fixed an error that occurred when using your hearthstone with the tradeskill window open.
* Converted the development repository to Git from Subversion.
* Removed the skill level and profit margin displays temporarily from the tradeskill window.
* Removed some redundant code.