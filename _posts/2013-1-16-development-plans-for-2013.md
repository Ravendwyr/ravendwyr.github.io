---
layout: post
title: Development Plans for 2013
categories: [Chinchilla Minimap, TradeSkillInfo, Broker uClock]
---

Here I will summarise the changes and updates I plan to make during 2013 once everything has settled down to some sort of normality.

There will be at least two new addons being released during the year; one in the next few weeks and the other in early June.  They are intended to be replacements for the two addons I recently discontinued and I will post more information about them when the time is right.

My current projects will also be receiving some love during 2013, with plenty of changes in mind.

**Chinchilla Minimap**

Mentioned in a previous news article and released prematurely in Version 2.5.10, Chinchilla's AutoZoom and WheelZoom modules will be merged together into one single Zoom module.  In their current state, the two modules conflict with each other which causes more problems elsewhere.  For example, there is a well-known bug where AutoZoom> often prevents the user from zooming back in using WheelZoom.  This will be just one of the many bugs fixed once the new Zoom module is complete.

The ShowHide and Position modules will also be receiving some love.  They will be rewritten from the ground up to remove a large amount of redundant code, and Position will finally be able to relocate the Arena and Battleground unit frames.  Support for these unit frames has been requested by the community for a long time and once the rewrite is complete, I will finally be able to begin working on them.

Overall the new code will be simpler, easier to maintain and will (hopefully) behave as intended without conflicting with itself.

**TradeSkillInfo**

Splitting the database into separate files was a success which now leaves me to work on the actual data.  Many recipes are displaying wrong ingredients or difficulty levels as these are forever being changed by major World of Warcraft updates.

Also, thanks to some new API that was recently added to the game, some of the library files embedded in TradeSkillInfo are now redundant. Once the database has been brought up to date, I want to start migrating over to the new API and eventually remove the deprecated libraries.

I have also been thinking about making a few more somewhat drastic changes; turning TradeSkillInfo's database into a separate "load-on-demand" addon, and re-indexing the database by spell ID number instead of item ID number.

Turning the database into a separate addon will speed up log-in times since the database won't be loaded into World of Warcraft's memory pool until it is needed.  Re-indexing the database will require a lot more thought and planning, but if I decide to go ahead with it the size of TradeSkillInfo's saved settings file will be reduced by over 50% and the database itself will become easier for me to maintain.  Considerable benefits for everyone, but potentially a lot of work.

**Broker uClock**

uClock itself won't change other than having its Interface number brought up-to-date for Patch 5.1.

What I have been considering is writing a separate "Lite" version of uClock.  It will simply be a databroker object with the text set to current local time and the tooltip containing the current date.  And that's it!  Ultra-lightweight, stripped down to the absolute minimum with zero configuration.

**The Blog**

I'm having a lot of fun pottering around with this website, but I don't want it to become Just Another Blog.  I want to add a jQuery-powered portfolio section where I can showcase each of my addons in their own individual page (or several pages, depending on the size of the addon).

I'm also toying with the idea of installing forums of some sort. We'll see.

**The Immediate Future**

At the moment there are no other known problems that I need to address (besides the ones detailed above) which allows me to focus on the replacement for TourGuide: Lunar Festival.  This year the Lunar Festival will start on January 27th and I hope to have this new addon available to the public by the 25th at the latest.

Soon after the release of the Lunar Festival addon, I will start working on TradeSkillInfo's recipe database and Chinchilla's zoom modules.

Be sure to report any problems you find in my addons.  Fixing errors and correcting bugs is always my top priority.