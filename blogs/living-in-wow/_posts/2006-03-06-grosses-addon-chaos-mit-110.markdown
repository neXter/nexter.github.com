---
comments: true
date: 2006-03-06 11:08:33
layout: post
slug: grosses-addon-chaos-mit-110
title: Großes AddOn Chaos mit 1.10?
wordpress_id: 1124
categories:
- Addons
- News
tags:
- Addons
- patch
- world-of-warcraft
---

Einem [Thread im US Forum](http://forums.worldofwarcraft.com/thread.aspx?FN=wow-realm-test&T=152330) zu Folge werden viele der beliebten AddOns nicht mehr nur einfach - wie sonst gewohnt - nicht funktionieren (und entsprechend gepatcht werden) sondern komplett geblockt! Ein Auszug aus der Liste:



> CT_Raidassist
Fishing Buddy
Mana Conserve
Discord Action Bars
Nymbia's Perl Unitframes
Decursive (bound to movement keys)
Gatherer
CT_RaidTracker
Quu's Spell Alert
FlagRSP





> {Add-On Name} has been blocked from from an action only available to the Blizzard UI. You can disable this addon and reload the UI. [Disable] [Ignore]



Dies liegt wohl an den neuen AddOn Bestimmungen und der umgestellten API. Mal gucken, was aus den beliebten AddOns dann wird. Ob es bspw. reicht, die nicht erwünschten Funktionen auszubauen (ManaSave bei CT_RA) oder ob noch mehr dahinter steckt udn sie gar nicht mehr funktionieren werden wir bald wissen...


***** Update *****

Liegt wohl momentan hauptsächlich an Funktionalität, die sich von sich aus ohen explizite Interaktion Dinge tun, bspow. indem sie sich an Aktionen wie "Spieler bewegen", "Maus klicken" etc. dran hängen und damit quasi ständig per Event ausgelöst werden:



> Blizzard disabled hooking some functions. Hooking these functions will result in the mod being blocked.

CT_RaidAssist hooks a function to check if the player is casting a spell through clicking in the game world. Removing this code piece makes it work just fine. It breaks some functionality though (namely the Resurrection Monitor).



Und offiziell:


> Addons and macros may not call or hook functions that initiate movement. (which I'm not doing)
You are no longer able to modify the Blizzard XML and Lua files. (which I'm not specifically doing... not overwriting the files, just overwriting a function)




***** Update 2 *****
Schöne Sammlung samt Fehlerlösung im [WoW Wiki](http://www.wowwiki.com/Broken_Addons_0.10:_Repair_and_Reporting).
