---
layout: post
title: TradeSkillInfo Updated to Version 2.2.6
categories: [TradeSkillInfo]
---

<script>const whTooltips = { colorLinks: false, iconizeLinks: false, renameLinks: false };</script>
<script src="https://wow.zamimg.com/widgets/power.js"></script>

Version 2.2.6 of TradeSkillInfo was released to the public a few days ago.  This is mostly a maintenance release, updating compatibility for World of Warcraft patch 5.1, "Landfall".

However, work on the database overhaul has begun and a lot of the files inside TradeSkillInfo have been moved, renamed or split into separate files.  Because of this, you must exit World of Warcraft completely before updating otherwise you will be flooded with errors.

The physical part of the database rewrite is mostly complete.  Some of the remaining files may get split up into smaller files but I won't be focussing on that.  Instead, my attention will instead be turned to the actual database content as well as how the data gets saved to the computer.  I have got some good ideas on how to move forward and I hope to start releasing more "alpha" packages for users to download and test in the next week or so (i.e., after I have finished exploring the new content in "Landfall").

Patch Notes:

* Separated TradeSkillInfo's built-in database into smaller files, one for each profession. This will make it easier for me to maintain.
* Updated the inscription database. Relics were deprecated when Patch 5.0 was released and most recipe skills produce Staff weapons instead.
* Fixed inscription recipes showing incorrect ingredients.  [Light Parchment](https://www.wowhead.com/item=39354/light-parchment) is now the only parchment type needed to create items.  The other parchment types were deprecated.
* Fixed [Forged Documents](https://www.wowhead.com/item=62056/forged-documents) showing up twice in TradeSkillInfo's browser UI.
* Moved the LibDataBroker-1.1 object code into a separate file and re-wrote it to make it more efficient.
* Added dummy code in preparation for upcoming database overhaul.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/tradeskill-info) or from [WoWInterface](https://www.wowinterface.com/downloads/info5473-TradeskillInfo.html).