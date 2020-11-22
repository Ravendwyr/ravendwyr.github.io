---
layout: post
title: First Few Updates for Patch 5.2
categories: [Chinchilla Minimap, TradeSkillInfo, SignOn, BottleCap]
---

Patch 5.2 "The Thunder King" for World of Warcraft was released three weeks ago and Patch 5.3 "Escalation" has already appeared on the public test realms!

I have been a very busy little bee since the release of Patch 5.2, buzzing around the new content and stinging any addon errors that cropped up.

Several of my projects have received a number of updates over the weeks including TradeSkillInfo, Chinchilla Minimap, SignOn and BottleCap. The website itself also got a new coat of paint and plenty of tweaks have been made behind the scenes.

**Chinchilla**

The new Zoom module is finished!

This new module replaces the older AutoZoom and WheelZoom modules, re-written from scratch with a few inspirations from SexyMap. The new code is far simpler and doesn't conflict with itself like the old code did.

You will need to exit and restart World of Warcraft after updating Chinchilla for the changes to take effect. If you don't, you will likely loose all zoom functionality until you do.

Patch Notes:

* Version 2.5.14
    * Fixed a positioning bug I introduced in Version 2.5.13. Whoops!
* Version 2.5.13
    * The Looking For Group minimap button can no longer be set to appear only when hovering the cursor over the minimap.
    * Fixed the positioning of the Looking For Group status popup when the minimap isn't in the top-right corner of the screen.
    * Fixed a leaked global variable.
    * Increased the mouseover fadeout time to 3 seconds (was 2 seconds).
    * Removed some unnecessary code.
* Version 2.5.12
    * Added Italian translations. Thanks to Curse user _YuSaKu_ for supplying these!
* Version 2.5.11
    * Merged the AutoZoom and WheelZoom modules into one Zoom module.
    * Switched back to AceTimer-3.0 instead of LibShefkiTimer-1.0.
    * Fixed some potential taint issues.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/chinchilla) or from [WoWInterface](https://www.wowinterface.com/downloads/info8394-ChinchillaMinimap.html).

**TradeSkillInfo**

I am still overhauling parts of the code and trying to keep the database up to date, but I am starting to admit defeat.

The database has always been maintained purely by hand, manually copying and pasting information from WoWdb and WoWhead into large files, but now that there is literally thousands of craftable items in the game it is time to start looking at automating the process somehow. I want to build some sort of data mining script that will build and update the database for me. It will make thing so much easier to keep on top of!

Other than that, I have been re-writing parts of the code to streamline them and make use of new APIs that weren't available before. I have managed to remove LibAbacus-3.0 and would like to remove LibBabble-Zone-3.0 and LibBabble-Faction-3.0 as well at some point.

TradeSkillInfo's database is largely up to date except for a few Tailoring and Blacksmithing patterns that were added in Patch 5.2, but they will be added eventually.

Patch Notes:

* Version 2.2.10
    * Added 6 of the new Reborn weapon Blacksmithing recipes.
    * Fixed skill level data for Zen Alchemist Stone.
    * Removed LibAbacus-3.0.
* Version 2.2.9
    * Completely rewrote the tooltip code from scratch to fix several taint issues users were experiencing.
    * Fixed a silly typo in the Ghost Iron Statue training project recipe.
    * Fixed skill level data for all Mining recipes.
    * Fixed skill level data for all First Aid recipes.
* Version 2.2.8
    * Added new recipe data for Engineering, Blacksmithing, Leatherworking, Jewelcrafting and Alchemy.
    * Fixed a bug with item tooltips in the crafting window due to Blizzard breaking tradeskill API.
    * Fixed a few typos.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/tradeskill-info) or from [WoWInterface](https://www.wowinterface.com/downloads/info5473-TradeskillInfo.html).

**SignOn**

SignOn had been left pretty much alone for the last few years.  It continued to work perfectly fine without the need for any updates (although it appeared as "out of date" in World of Warcraft's addons menu) so I pretty much let remain that way until recently.

Curse user Profalbert uploaded a patch to my repository on WoWace.com which added a significant new feature; redirecting all logon/logoff messages to a separate chat tab. Many users have a chat tab dedicated to guild chat but until now had to endure all system messages to keep an eye on who logs in or out of the game. With this new feature they can now enjoy only seeing logon/logoff messages in their guild chat tab and keep the rest of the system messages somewhere else.

I really liked this idea and with profalbert's permission I cleaned it up and brought SignOn back up to date.

Patch Notes:

* Version 2.4
    * You can now redirect logon/logoff messages to a different chat tab.
    * Updated compatibility for Patch 5.2.
    * Fixed some potential talent frame taint issues.
    * Fixed the :colour flag. It is now truly random every time.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/sign-on) or from [WoWInterface](https://www.wowinterface.com/downloads/info11801-SignOn.html).

**BottleCap**

After a long hiatus, BottleCap is back!

It continued to work more or less ok, although it wasn't able to monitor the new Instance or Battle.net chat channels that were added in recent patches, and it's Verbose Mode feature broke some newer chat links including the Encounter Journal and Battle Companions.

The biggest change was the removal of Ignore Mode. It caused more problems than it solved and it has been axed from the addon.

I must also take this opportunity to thank Mr John B. from the Netherlands for his donation and support for BottleCap.  All donations are gratefully received and help to fund continued development for your favourite addons!

The capslock prevention addon you knew and loved is back from the dead and is now fully compatible with Patch 5.2!

Patch Notes:

* Version 3.2
    * Updated compatibility for Patch 5.2.
    * Added monitoring support for Instance, Instance Leader, Battle.net Whisper and Battle.net Conversation chat channels.
    * Added "/bottle" chat command to open the options window.
    * Fixed clickable links for Encounter Journal spells and Battle Pets in monitored channels with Verbose Mode enabled.
    * Fixed some potential talent frame taint issues.
    * Removed Ignore Mode.
    * Removed options to monitor Battleground chat channels since they were replaced with the Instance channel.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/bottle-cap) or from [WoWInterface](https://www.wowinterface.com/downloads/info10877-BottleCap.html).