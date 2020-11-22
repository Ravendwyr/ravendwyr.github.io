---
layout: post
title: TradeSkillInfo Updated to Version 2.2.18
categories: [TradeSkillInfo]
---

<script>const whTooltips = { colorLinks: false, iconizeLinks: false, renameLinks: false };</script>
<script src="https://wow.zamimg.com/widgets/power.js"></script>

I am a bit behind with posting news updates here, but things are calming down now and I hope to get on top of things soon.

Today, I released v2.2.18 of TradeSkillInfo.  This version includes a lot of updates to the recipe database and finally fixes a few bugs that I have been tearing my hair out over.

Please note that v2.2.18 will be the final stable update before a database overhaul that I have been planning for months.  Unfortunately, this does mean that TradeSkillInfo's saved settings WILL BE RESET as of r688-alpha and onwards.  With Warlords of Draenor officially going live at midnight on November 13th, now is the time to finally put my plans into action.

If you do not want to have your settings reset, then please set your Curse Client installation to download "release" type packages instead of "alpha". The next big stable release package will be v2.3.0 and is planned for release on November 10th.

I apologise for the inconvenience the reset will most likely cause, but due to the nature of the changes there is no possible way to convert existing settings or provide backwards compatibility.

One of the biggest changes that will be made during the overhaul, and definitely one I am really excited about, is that maintaining TSI's recipe database is now 100% automated thanks to a datamining script gifted to me by Curse user Bodar.  Up until now, the database had been maintained purely by hand.

Also, with thanks to the new database layout, the much-requested feature to delete characters from TSI's settings will finally be able to implemented.  The previous layout did not allow this to happen easily which delayed implementation far longer than anyone wanted.

Finally, TradeSkillInfo's development repository will remain as Subversion for the foreseeable future.  Those of you who use TortoiseSVN (or similar programs) will be happy to know they can continue to do an "svn checkout" to download the latest version of TradeSkillInfo.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/tradeskill-info) or from [WoWInterface](https://www.wowinterface.com/downloads/info5473-TradeskillInfo.html).  If you come across any problems feel free to get in touch.

See you in Draenor!

<strong>Official Changelog:</strong>
<em>v2.2.12 to v2.2.18</em>

* Marked as up-to-date with Patch 6.0.3.
* Fixed co-ordinates for [Nessa Shadowsong](https://www.wowhead.com/npc=10118/nessa-shadowsong).
* Fixed problems with A TON of recipes.
* Fixed a bug that caused the Browser UI to permanently lock up when it tried to display a deprecated recipe.
* Changed the QuickSearch feature to be off by default.
* Updated the Browser UI to use the new GetSpellDescription() API instead of creating a custom tooltip to scan through.
* Updated keybindings to use the "AddOns" category in the new Key Binding UI.
* Updated various translations.
* Removed function hooks for TradeSkillHD as they are no longer needed.
* Removed tekConfig libraries.
* Removed redundant code.