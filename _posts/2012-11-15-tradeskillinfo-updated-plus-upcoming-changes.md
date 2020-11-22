---
layout: post
title: TradeSkillInfo Updated plus Upcoming Changes
categories: [TradeSkillInfo]
---

TradeSkillInfo has been updated to Version 2.2.5, bringing with it a few fixes to its database and a few changes behind the scenes.

There is still quite a lot of incorrect and missing information in TSI's database and I'm hoping my planned database rewrite will make it easier to manage.

Currently the database is one huge file.

As in, ~520 kilobytes huge.

It has grown to the point where it has become difficult to maintain and daunting for my userbase to contribute patches. To address this,  I plan to split the database into several smaller files, one for each profession, and put them into their own directory inside TradeSkillInfo's install directory. This, in theory, will make maintenance far easier than it currently is.

I also eventually want to remove several deprecated libraries that TSI currently uses, including Lib-BabbleZone-3.0 and Lib-BabbleFaction-3.0. Blizzard have added some new API functions that made these libraries pretty much redundant. I currently plan to begin re-writing parts of TSI to use the new API after I have finished messing about with the database.

If none of this makes any sense to you then you have nothing to worry about and you will likely not notice any difference after updating TSI. However some of my users are a bit more technically minded than Average Joe and like to know what's going on.

As always, if you have any feedback or questions regarding this addon then please don’t hesitate to get in touch. User feedback is greatly appreciated and helps your favourite addons evolve!

Patch Notes:

* Fixed a few incorrect skill levels for Inscription inks and First Aid bandages.
* Numerous behind-the-scenes preparations for an upcoming database overhaul.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/tradeskill-info) or from [WoWInterface](https://www.wowinterface.com/downloads/info5473-TradeskillInfo.html).