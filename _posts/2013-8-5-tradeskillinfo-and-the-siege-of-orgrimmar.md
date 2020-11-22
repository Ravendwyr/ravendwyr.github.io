---
layout: post
title: TradeSkillInfo and the Siege of Orgrimmar
categories: [TradeSkillInfo]
---

I have recently been made aware that the format of tradeskill hyperlinks will be changing in Patch 5.4, "The Siege of Orgrimmar".

Tradeskill hyperlinks are the clickable yellow profession names you often see in various chat channels (i.e., [Engineering]) which present a list of the craftable items that player can create.

The hyperlinks are being simplified slightly and will provide less information inside them:

`5.3 format: |Htrade:(playerGUID):(spellid):(rank):(maxrank):(databits)|h[profname]|h`

`5.4 format: |Htrade:(playerGUID):(spellid):(??)|h[profname]|h`

Most notably, the (databits), (rank) and (maxrank) fields are being removed entirely and all data will be fetched dynamically from the server based on player GUID in the link.  The contents of the (??) field is usually a three-digit number and the relevance of this field is not yet known.

The implications of this change are that most addons that parse the (databits) field of tradeskill hyperlinks will need changes for Patch 5.4.

So what does this mean for everyday users?  Probably not much, but addons that provide "All Recipes" hyperlinks, such as Professions Vault and Ackis Recipe List, will need to remove that feature as those links can no longer be created.

Thankfully, TradeSkillInfo and its features should be completely unaffected by this change as TSI does not use tradeskill hyperlinks to manage recipes.  That said, I cannot guarantee that TSI will be error free when Patch 5.4 goes live as I have not downloaded the current PTR.  I will keep an eye out for any bug reports that come in and act on them accordingly.