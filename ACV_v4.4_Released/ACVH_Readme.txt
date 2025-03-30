Prenotes:
- IMPORTANT PRENOTES:
  For non-legit users, you MUST:
    0. keep in mind that you WILL crash now and then, so take backups regularly !
    1. enable (all) scripts while NOT ingame (iow while in Main menu, Inventory or Map for example)
       Tip: FT to a "non-city" location first, and then draw your bow for a moment (which accesses the inventory) (and then press [ESC])
            Now, switch back to CE and start enabling all scripts (and thereafter disable those you'd like disabled presently)
    2. if certain scripts do not enable immediately, then you'll need to Fasttravel to a different location first!
       That said: if this occurs, the game tends to crash eventually; usually after some FT/cutscene action/etc...
       Important: do not try to keep clicking the script_box; it will lead to certain game crash...!
    3. Tip: do not active while in crowdy locations (such as Raventhorpe, any city, etc...)
    4. Tip: play the game a few minutes before activating any script...
       (failing to do so will simply crash the game almost instantly)

  Other:
    Reported back by #VixHexven:
    5. The game crashes at certain events while in Ragnarok (with eg Godmode enabled) !
       Workaround: change the CE debugger to 'windows debugger' ~ [Edit ~ Settings ~ Debugger Options]
       (note: other tables might depend on this option being set to VEH; keep this in mind !)
    6. During raids, certain enemies can not be killed (seem to have godmode enabled); cause not yet found...
    7. In 'New Game Mode', you might need to re-enable certain cheats/scripts to pick up correct value(s) again.
       (such as Adrenalin)

- This version makes use of features introduced in CE v7.1x or higher...
- Best practise is to load the table AFTER your save game has fully loaded...
- You should only work with 'normal color' cheats (do not touch 'greyed' info)
- When returning to the main game menu, best is to disable the main script first!
- FastTravel (and Cutscenes) will 'reset' data structure pointers. Whenever this happens,
  you must re-enable selected (sub)options again, if needed...
- All values (pointers) will be collected while "active" as player.
  (iow not while in 'ESC' or 'TAB' mode)
- Also - where appropriate - 'greyed' structure pointers are shown, and these must contain a value to work properly !
  (if zero, switch back ingame to have them collected)
- If you initially selected an incorrect game_exe, you might be prompted with a warning upon selected the correct exe.
  You can safely ignore this message, and the table will load fine thereafter...
- After returning back to the Title Screen, you should disable all cheats (using [Ctrl+F12]) !
  (or else there is a good chance of crashing the game upon returning ingame...)
- Always make manual backups of your save(s) to avoid possible loss (~ corruption/locked player/etc)
  You have sole/full responsibility over your gaming environment.


Important:
Now, when performing any form of teleporting, 'Ignore Fall Damage' will always be enabled automatically !
(iow do not forget to disable it later on...)


* Player Status:
- Health: can be locked if needed
  Note: to force a 'desync', just set the player's value to '-1'
- Godmode [Ctrl+G]: used especially during Freeroaming...
- Invisible: you will become undetectable
  (even when already in conflict, you still become invisible instantly...)
- Infinite Consumables: (most) resources (such as silver, arrows, etc) will not decrease when consumed
- Adrenaline: can be locked if needed
  Note: 'lock' it to show additional features (no extensive testing performed though)
        (do not touch 'Consumption' - see it as a percentage value - as it will crash the game !)
- Enemy 1-Hit Kill/Defense (you can change its initial/maximum value)
  * Health: enemy's health will be set to 'Health Max'
  * Defense: resets enemy's defense (bar above health)
  * God Mode Friendly (should cover most Friendlies/NPCs)
  Notes:
  a. should cover most enemies (incl Bosses). However, if you do come across a situation whereby the script
     does not act accordingly, report back...!
  b. uses Faction to identity entities; however the game is not always consistent in that certain "enemies" are defined as friendly
     (and vice versa)
- Stamina, Stamina horse, Oxygen: can be locked if needed
- Ignore Fall Damage: you will not die, falling from any height (primarily used for teleporting purposes)

* Inventory: edit accordingly, but keep most values in line with game "expectations"...
  To collect the current inventory values, just click 'Collect Resource/Item Values...' once.
  (if nothing seems to update, return ingame, draw your bow for a moment. Switch back to CE and dis/re-enable 'Inventory...' again)
  Notes:
  - you should/must always 'collect' first before editing any values (~ ensures correct values are accessed)
  - edited values will only be updated after leaving, and then going back to Inventory
  - only items which are already "known" to your current game status, will show correct values
    (f.e. if you have no arrows, then it will always show '??' as value)
  - important: do not change any value that does not match...!
  - if some values no longer match, just run the script again
  - the 'Full Inventory' list is now sorted by 'Type/Category'.
  Tip: if the script does not enable immediately, FastTravel first (which could also solve the 'offset too big' error)

Options: 
  1. Collect Info: gets values for resources, crafting materials, etc (see subcategories)
     (only items which have no zero value !)
  2. List Resources: lists abovementioned info, and allows you to change an item/items total value.
  HowTo:
  a. set all values to a "maxQuantity" value: simply click the 'Set to MaxQuantity...' button (red top-right button)
     (see greyed '(pBhvAssassin) - Base' to change this MaxQuantity value)
  b. copy/paste this list: click the 'Copy list...' button (top-right button); then paste it into Notepad
  c. edit specific item: select it in the list, then click the 'Edit item values...' button  (top-right button)
     1) double-click the 'Address: Value' column
     2) Total: set it to a new value (and [Enter])
     3) to get the list visually updated, you must run 'List Resources' again...

  3. List Full Inventory: gives a list of ALL inventory items; and also allows you to edit its 'Total' value
     To edit 'Total' value, just select an item in the list and then click the [Edit item] button (in top_right corner)
     In this new/small window, just double-click the 'Address: Value' field to change/update its value...
     Note: the 1st time you click the button, it might return a 'List index (x) out of bounds' error;
           just ignore/close that message and click again...

  4. List Full Inventory (All): same as above, but also includes items without known descriptive.

  5. List Duplicates: gives an overview of duplicate items, and allows you to easily remove these from your inventory
     To remove/delete these items, just click the [Remove items] button (in top_right corner)
     (you will be asked to confirm deletion, and instructed on how to proceed next...)
     Notes:
     a. if this list does not report all items, then also see: [Inventory Editor - HowTo remove duplicates] pdf...
     b. if you rerun 'List Duplicates' afterwards (and before saving/loading), you'll notice that the 'Total' has been set to '0'
     c. duplicate gear/weapons will always restore to default quality...!
     Important: always make sure to have a Save backup at hand !
   
  6. Special - Full Item List: gives a list of all items (also those not present in your current inventory
     Notes:
     a. this list can also be built, while using the 'Report Seperator' (for ease of Excel importing for example)
     b. when entering '*-' (without quotes), you'll get a variant (which can be used in conjunction with the 'Editor')
     c. when entering '*+' (without quotes), you'll get a variant (which is used in this table to show the descriptives)

  7. Special - Item Sets: lists items per appropriate set (~ pack)
     Notes:
     a. this list can also be built, while using the 'Report Seperator' (for ease of Excel importing for example)
     b. when entering '*-' (without quotes), you'll get a variant (which can be used in conjunction with the 'Editor')

     HowTo export 'Special Lists':
     a. set '1. Report Seperator' to your preferred (1-char) seperator ('~' is a good character as rarily being used)
        (leave/set it blank to print standard reports !)
     b. build/run the list
     c. either copy the list to the clipboard (using the appropriate button in top_right window); 
        or directly import into Excel using [Paste ~ Use Text Import Wizard] (while using 'your seperator' only !)
     Tip: see also: [ACVH_ItemList_Compare.pdf]

  General note: all lists can be copied to the clipboard !

* Teleport & Coordinates:
> Teleport to 'Map Waypoint': (you must enable this script first)
Prenote: save regularly while extensively using the teleport feature !

When selecting a location on the map, teleporting to that location should be fine.
However, keep in mind that Player can sometimes drop from a greater height (and therefore will/could die/desync).
To avoid this altogether, simply enable 'God mode' first...

1. Open the map and select a(ny) location with your preferred Waypoint number
   (disenable the/any Waypoint on the map first, if needed)
2. Press [Ctrl+P] ONCE (sometimes twice) while still in the map view...!
   (if done correctly, your player's icon should move to the new location)
3. Press [ESC] and Player should now teleport to that particular location
Tip 1: best tactic is to always use/stick_to the same Waypoint number !
Tip 2: You can also use Raven's waypoint; for example to teleport to specific surfaces (such as rooftops)
Tip 3: NEVER select/teleport_to the 'Drinking' icon as this seems to hang the game ?!
Tip 4: wait in_map for the 'loading_icon' to finish before returning in_game...

Notes:
a. If you wind up in some structure (like rocks, hills, trees, building, etc), try to teleport
to a different location first; or use FastTravel.
Tip: you can also try FreeRoam... (press [Esc] first before activating the script !)
b. Avoid pressing [Ctrl+P] altogether when NOT in the Map view; results can be unpredictable...
   (with a good chance of game crashing)
c. If you fall "through the surface", immediately press [ESC/Tab], increase your Z-value (high enough, e.g. {600}) and you should
   be back on/above the surface (or simply use FastTravel). Or enable Free Roam, and then ascend...
d. This game makes use of 3 waypoints (Sets 1~3) to choose from (numbered from 0 to 2 internally).
   You can consult each of them coordinates via 'All Waypoint Coordinates...'

> Free Roam (also check out Help function)
Once enabled, you use your mouse to steer in a particular direction, and use Numkeys [8] (= forward)
and [2] (= backward) to move about.

Major FreeRoam tips:
a. before ending FreeRoam, try making your player "stand" first. Basically, you keep him/her in the air until s/he starts
   "waving his arms", then descend to a surface to get your player stand clearly... If you press [F10] now, things should be fine.
b. keep your roaming distances "short". The further you move, the higher your player seems to get "catapulted" ?!
   (unless you stick to pt. a.)
c. if you get "locked" in/at a certain position, then you'll need to disable 'godmode' to get your player killed eventually... !
   (in case everything else fails)

Notes:
1. upon enabling free roam, you must FIRST move forward a bit in order for the game to pick up...
(in some cases, you'll need to push both keys - eg forward and NumKey '8' - at the same time for a moment)
2. avoid moving through structures, as this seems to "confuse" the engine (~ then usually only able to continue in one particular
direction). Drop down to a surface, or move your player in such a way that he changes posture (which should solve this issue)
3. you can hold a key to speed up things (you could also change a 'stepValue' accordingly ~ see [Script values])
4. you can end the roaming-session either using [F10] (or disabling the script) or [F12]
(which should bring you back to your start position). In the lather case - when unsuccessful, enable 'Save & Restore Coordinates'
and press [F12] again...
5. if the player seems to get "out of sight" simply use your mouse to look (around) from a different angel,
which should (eventually) give focus back onto your player... (and/or use ascend/descend keys)
If such actions do not seem to work and/or the player is "locked" in a particular direction, then end the roaming session
and continue from there onwards...
Tip: while ascending/descending much, give the game "some" time to update the camera position. Iow keep the player close in sight
by regularly stop moving, and bringing your view back into the horizontal plane. The camera position should then return to the same level...
6. if you start roaming while stuck inside a structure, then you'll need to move some distance away first before ending roaming !
(or else your player gets pulled back to his original position)
7. your player can change of posture depending on when/where you start roaming; or because of passing through certain structures.
If you fail changing to a "normal" falling posture, performing a FastTravel will solve this...
8. If your player changes/remains in "hanging position" then disable Free Roam and try [Shift+'Wall Eject'] to drop back to surface...
If all fails - or you loose patience - just FastTravel...
9. TIP: before starting effective roaming, ascend a bit (~ make sure you look up a bit to get best effect). This way you'll avoid a possible change in posture of your player ! Also: you might need to move forward first in order for the game to pick up...

Important: occassionally, the coordinates system goes into "overdrive" making your player uncontrollable.
           Some experience shows that one can try melee-ing (or some other action), and then try to teleport to another location.
           However, in most case, you'll have to reload your last save !
           (or disable 'God Mode' to get you killed)

> Cam Distance: change the distance towards the player's location (could also be called FOV)

> Save & Restore Coordinates: use [F11] (save current coordinates) and [F12] (restore saved coordinates)
  to teleport back to a specific location.
  Notes:
  1. you have the option to either reset coordinates after teleporting (to avoid inadverted teleporting ~ set by default);
     or just keep them active.
  2. you 'enable' this feature by selecting the appropriate option_choice in the 'Value' column...
  3. the feature also takes 'Drop Height' into account (to avoid possible collisions)

* Miscellaneous:
> Raid Alarm Level: allows you to lock alarm level during river raids (unlock before leaving...)
> Timer Hugr Power: sets the time range for any hugr power
  (note that you can "extend" the timer by just pressing the same power again...)
> Timer Helfire: you can change the 'endtime' by increasing the (integer) counter (basically its highest digit(s))
  Notes:
  a. you can buy the 'Silent Assist' favor at some point to disable this timer altogether
  b. I might create a more userfriendly cheat (see ACU) in due time...
> Mastery Challenge: allows you to easily obtain all gold medals

> Time Of Day: set/lock time of day.
  > Weather: allows you to dis/enable certain weather features (use any value between 0~1)

> Progression Data: allows you to edit appropriate values
  > Experience Points: best work with Experience values only to increase/add Skill Points...
  > Charisma Level: increments per 1 point; and every 4 points will level up your charisma...
  > Settlement Level: only edit if game behaves buggy (or you want to - temporarily - "force" some quest activation)
                      (increments per 100 points)
> Progression Skills: allows you to edit skill & mastery points
  Note: ingame, it will show 'Power' + 1



* [Tools] menu:  (see top menu-bar choices)
> Compact View:
allows you to show/hide the typical CE interface (Compact (default) = show only the cheats-list)

> Select & Launch Your Game...: allows you to launch the game directly from this table.
The 1st time, you'll need to find/select your game's (sub)folder. Once the game has launched - and you want to keep its (sub)folder location - you can/must save the table manually to keep that setting permanently.
(see also 'Cheat table settings' below)

> Disable All Cheats: will disable all cheats, and unlock any locked values
  (you could use this between mission/save/etc-loads when crashes seem to occur at that moment in time)
  Note: [Ctrl+F11] = unlocks 'locked' values only ~ [Ctrl+F12] = disables all cheats (incl scripts)

> Show Table Name: will - in most cases - only show correct tablename when game has not yet been launched/attached.
  v7.1+ users will/should always get the correct tablename shown !

> Errors & Settings:
§ Error Statistics...: logs errors handled by CE (basically handling possible crashing);
                       and all values should remain at '0' normally

§ Cheat table settings...: (as user you can change certain - default - settings here)
- Browser: upon clicking the 'Info' button, this broswer will be launched with a search string
  to find the related game topic @FRF (it should use your default search engine)
- Compact View Mode: set your preferred default startup
- Color: will be used as background color in the cheat list overview
  (you can use one of the online 'Color picker' tools to get a proper (hex)value)
- Game' exe and (sub)folder: exe used for 'auto-attach'-ing; and opening the proper game folder via 'Select & Launch Your Game'
  Note 1: the 1st time that you use this feature, your game folder_location will be copied here. However, you must save
          the CE table manually in order to keep this setting permanently.
          Also: clear this info in case you have changed your game location thereafter... (or update it manually here)
  Note 2: some tables offer a feature to export/save certain reports to a file.
          In such cases, the "export function" will look for its 'Report export location' here.
          (if you get a '... is undefined' error message, you'll have an incorrect path reference filled in here !)
          * <game> : refers to your game location (entered in previous field above)
          * <table>: refers to your CE table location (see also: [Tools ~ Show Table Name...])
          * 'any existing folder' (eg: C:\TEMP\)

Note: use 'apply above changes...' to check out your changes first, before saving !

Important: if you want to keep any change(s) permanently, you must manually save the table, quit CE and load up the table again!

- Developer tools... (do not use, unless at your own risk)
  Important: this table depends on '(game verification...)' set properly. Iow do not change this setting !
- Maintenance scripts... (do not use, unless at your own risk)
  (allows table author to manage 'system' settings more easily ~ again, not to be used by gamer at all !)


ps: you can change/introduce hotkeys via CE's 'hotkey' feature
    (eg: [Ctrl+G] = dis/enable God Mode)
