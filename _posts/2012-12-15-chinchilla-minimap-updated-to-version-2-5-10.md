---
layout: post
title: Chinchilla Minimap Updated to Version 2.5.10
categories: [Chinchilla Minimap]
---

This will likely be my last update for 2012, as tomorrow is my birthday and Christmas is 9 days after that.

Chinchilla Minimap has been updated to Version 2.5.10. This update was made to fix an error spotted by user Kamata on Curse.

The error didn't happen very often thankfully as it was only being caused when a font registered with LibSharedMedia-3.0 became unavailable (for example, the addon that registered the font with the had been disabled or uninstalled). It was mostly my fault as I didn't read the API documentation for LibSharedMedia-3.0 properly in the first place.

Version 2.5.10 also includes some unfinished work-in-progress; I had begun to merge the AutoZoom and WheelZoom modules together into one simple Zoom module. While functionally sound, the new Zoom module does not yet have any in-game configuration. Users with enough knowhow can modify Chinchilla's saved settings manually but I can only provide limited support if they choose to do so.

I wanted to hold out and release Version 2.6 in the new year with the new and improved Zoom module but I also wanted to fix the reported error as soon as possible. This trade-off gives me an excuse to continue poking Chinchilla's code into 2013 and beyond!

Patch Notes:

* Fixed an error caused when a "shared font" became unavailable.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/chinchilla) or from [WoWInterface](https://www.wowinterface.com/downloads/info8394-ChinchillaMinimap.html).