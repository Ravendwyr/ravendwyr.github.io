---
layout: post
title: MogIt Highlighter Updated to Version 1.3
categories: [MogIt Highlighter]
---

My first official project update for 2015, I bring you a new version of MogIt Highlighter.

Version 1.3 is a maintenance release with no new features, but it does include some extra safeguarding against potential UI taint issues.  I never received any reports of taint errors but it is better to be safe than sorry.

The new safeguard comes in the form of `LibButtonGlow-1.0`, which is also included in the latest versions of Bartender and WeakAuras.  This embeddable library provides a completely custom glow animation for addons to use, as using Blizzard's default glow animation or even its template can cause taint errors.

What does this mean for end users?  Not much, except that addons that use the library are taking steps to prevent taint and UI lockups wherever possible.

The new version of MogIt Highlighter is now available to download from [CurseForge](https://www.curseforge.com/wow/addons/mogit-highlighter) and requires [MogIt](https://www.curseforge.com/wow/addons/mogit) in order to function.  As always, if you have any questions or feedback then please do not hesitate to get in touch.

Enjoy!