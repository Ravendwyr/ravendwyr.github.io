---
layout: post
title: Chinchilla Minimap Updated to Version 2.6
categories: [Chinchilla Minimap]
---

After being left in "alpha" status on Curse since Patch 5.2 came out, Chinchilla Minimap has finally been given a new public release version.

While I haven't yet been able to finish working on everything that I'd like to, this release includes several important fixes to bugs introduced with Patch 5.4.

There have also been a number of fairly large changes behind the scenes, some of which I felt were needed but may prove controversial.

This includes the deletion of the QuestTracker module.  This module was deemed "out of scope" of Chinchilla's development goals and has been removed, but the options to show/hide the quest tracker's "Objectives" header text and collapse button proved to be popular features and these have been brought back as options in the Appearance module instead.

You can download the updated version from [CurseForge](https://www.curseforge.com/wow/addons/chinchilla) or from [WoWInterface](https://www.wowinterface.com/downloads/info8394-ChinchillaMinimap.html). As always, if you find any errors or want to provide feedback, please do not hesitate to get in touch!

<strong>Official Changelog:</strong>
<em>v2.5.14 to v2.6</em>

Core
<ul>
	<li>Flagged as compatible with Patch 5.4.</li>
	<li>Removed large chunks of useless code.</li>
	<li>Options window size increased slightly.</li>
	<li>Options for modules are now hidden when the module is disabled.</li>
	<li>Fixed "this function is already hooked" errors when addon is disabled.</li>
</ul>

Appearance
<ul>
	<li>Fixed a long-standing bug causing the "button border alpha" feature to not work at all.</li>
	<li>Button border alpha feature extended to work with buttons created by LibDBIcon-1.0.</li>
	<li>Minimap strata options simplified to Low, Medium or High.</li>
	<li>Default minimap strata setting changed to Low to match Blizzard's default setting.</li>
	<li>Removed AceTimer-3.0 from the module.</li>
	<li>Removed large chunks of useless code.</li>
</ul>

Compass
<ul>
	<li>Blizzard's default compass ring is now invisible instead of hidden.</li>
	<li>Removed large chunks of useless code.</li>
</ul>

Position
<ul>
	<li>Boss frame movement temporarily disabled pending code overhaul.</li>
	<li>Looking For Instance status popup should no longer get stuck behind the minimap.</li>
</ul>

QuestTracker
<ul>
	<li>Module deleted.</li>
	<li>Options to show/hide header and collapse button moved to Appearance module.</li>
</ul>

ShowHide
<ul>
	<li>UI elements supported by this module are now invisible instead of hidden.</li>
</ul>

TrackingDots
<ul>
	<li>Blip maps updated to Patch 5.4 layout, adding new icons for Timeless Isle hostiles/objects.</li>
</ul>