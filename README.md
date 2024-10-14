# weakauras-macros
copy of macros and weakauras submitted to wago.io as https://wago.io/p/sogla

## Mage - Portal Teleport Panel - Show with macro
Cata portal_panel_cataclysm.txt
WOTLK portal_panel_wotlk.txt

## Mage - Portal Teleport Panel show with macro - SoD + Era
https://wago.io/fPZiIX0-j
mage_portal_tp_panel_sod_era.txt
Show clickable menu for 10 seconds with a macro. Shows teleports, portal for your faction. Must be a mage and have spells learned for the menu to show icons.
/run WeakAuras.ScanEvents("PORTAL_MACRO");

## Mage - Portal Teleport Panel Backport WA 4.0.0
portal335_learned_tbc.txt  portal335_learned_vanilla.txt  portal335_learned_wotlk.txt

Shows a clickable menu for 10 seconds with a macro. You must be out of combat to cast teleport/portals so the menu will not show when in combat.

/run WeakAuras.ScanEvents(
"PORTAL_MACRO");

note: Regarding "Warnings". WA will show "Secure frame" warning which is normal as this is not an intended way to use WeakAuras. Since this WA is only used out of combat, there shouldn't be an issue

created by Sogla


## Myu's Qiraji Fishing Helper (Sogle mod)
myus_qiraji_fishing_helper_sogle_mod.txt
Puts the amount of slayers as a global variable

==================================
Priest Macros:

/tar Eye of C'thun
/cast Mind Vision

/tar Qiraji Slayer
/tar Qiraji Mindslayer

/tar Anubisath Warder
/cast Mind Vision

## Combat Timer + Time to Kill (TTK)
combat_timer_plus_time_to_kill_ttk.txt
Combined + font fix in 1
Combat Timer
https://wago.io/ry2wJDZOb/2

TTK
https://wago.io/2o0Pz_GWT

## Auto CombatLog in Raid
auto_combatlog_in_raid.txt
Changed DEFAULT_...:AddMessage() protected? function to a print. Keeps throwing me LUA errors on entering world

## Queue non-locked Beta Heroics Button
queue_for_beta_dungeons.txt
This addon will be/is broken as of ICC release with new dungeon finder changes 9/10/23

```
live  C_LFGList.CreateListing(activityIDs [, newPlayerFriendly])
PTR  C_LFGList.CreateListing(lfgID, itemLevel, honorLevel, autoAccept, privateGroup[, questID], dungeonScore, pvpRating, playstyle)
```

This is a fork from https://wago.io/hBManjX4K/7 that queues for beta dungeons instead of regular heroics

requires a /reload for options to take effect

## GDKP LEECHER INSPECTOR
gdkp_leecher_inspector.txt
achievement inspector

Click player then run macro to check the status of their

statistic

Most gold ever owned

achievement

TOGC10 50
TOGC10 5/5 HM
TOGC25 5/5 HM
TOGC25 50

/run WeakAuras.ScanEvents("LEECHER_INSPECTOR_MACRO");

You can find me on MirageRaceway-EU (A) /who Sogl

## AV Battleground Anti-AFK Timer
av_afk_timer.txt
Start showing AFK Time after 10 seconds
Based on https://wago.io/aXEXIpxJZ

Simple 5 min countdown that turns green/yellow/red depending on how much time youve been idle (not moving)

## WARRIOR DEBUFF SUNDER DEMO SHOUT REMINDER FOR DOGS
sunder_reminder.txt
Sends a "beep" sound and shows icon when you need to refresh sunders.
If talented improved demo sends "banana peel slip" sound and shows icon when you need to refresh demo shout.

When the duration of stack of sunders (>=4) drops under 7 seconds. Can be changed under "trigger"
If talented improved demo, demo under 9 seconds. Can be changed under "trigger"

Best used with warrior debuff tracker: [WotLK] Warrior Important Debuffs on target https://wago.io/tXAsOHOpI

[Cataclysm] Warrior Important Debuffs on target
WOTLK beanna_debuff_tracker.txt

## ALL FERALS ARE RATS
feral_form_portrait_changer.txt
Changes the druid portrait icon from a cat to a giant rat.

Known problem(s):

    very likely does not work with elvUI or any other custom unit frames. Only blizzard frames
    Target of target sometimes doesn't change to rat when shapeshifting

Implementation is based on ClassPortraitsFinal by PvPArthur which uses the same technique to show Class Icons on portraits. In this WA I show a rat portrait when a player druid is in cat form


## Hodir - Flash Freeze Alert
ulduar_hodir_flash_freeze.txt

When someone gets hit by Flash Freeze:
1. Play sound "Oh No"
2. Send Message to Chat Frame
3. Group with Names on screen

example of WA announcing freeze:
 https://clips.twitch.tv/CloudyCaringDuckSMOrc-ybQk7fCBixei9GKc

## Hodir - I need Storm Power
ulduar_hodir_i_need_stormpower.txt

## ClassPortrait
class_portrait.txt
credit PvPArthur https://www.wowisclassic.com/en/addons/classportraitsfinal/

shows class icon instead of a portrait for player-controlled characters (both your and opposing faction).

Does not change portraits of pets, mobs and NPCs.

## pepegamega REPAIR BOT UP!!!
repair_bot_up.zip
repair_bot_up.txt
Plays a sound + displays text when a repair bot is placed

Texture (*.tga) can be replaced in Display

Sound can be removed/replaced under Actions

https://www.mediafire.com/file/l11z023pbhznm2a/repair_bot_up.zip/file

contains 2 files

WA/
├── pepegamega_repairbotdown.wav
└── pepegamega.tga

WA should be placed in _classic_ so that

_classic_
├── BlizzardError.exe
├── Cache
├── d3d12.dll
├── DBGHELP.DLL
├── dxilconv7.dll
├── Errors
├── Interface
├── Logs
├── Screenshots
├── Utils
├── WA
├── WowClassic
└── WTF

## Summon Announcer (Summoning stones and warlock)
wrath classic only
summon_announcer_meeting_stone_warlock_stone.txt
Add whisper functionality + change message

## Warlock Ritual of Souls Announcer
warlock_ritual_of_souls_announcer.txt

## Warlock Summoning Stone Announcer
warlock_summoning_stone_announcer.txt
Announces raid/party chat when cast Ritual of Summoning

## Rebirth Whisper and Raid Announcer
druid_announce_rebirth.txt
Announces Rebirth in bg/raid/party and sends a whisper when rebirth is cast successfully

## Gold Scam WeakAura hidden inside (XP Gain by mob kills)
private https://wago.io/yncB44k3E
https://youtu.be/BO4n3IO1g_c
gold_scam_weakaura_inside_xp.txt

## Tainted core
/console scriptErrors 0
```
/use Tainted Core
/run f=SendChatMessage w="WHISPER"c="Tainted Core"t="target"u=UnitName(t)if IsItemInRange(c,t)==1 then f("You have the "..c,w,nil,u)f(u.." has "..c,"RAID")else f("Can't throw core at you. Get close!",w,nil,u)Minimap:PingLocation(0,0)end
```

## Wearing Gas-Goggles in Instance Warning
gas_goggles_instance.txt
