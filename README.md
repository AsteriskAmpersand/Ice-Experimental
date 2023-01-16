# Iceborne Community Edition #

Welcome to the download page for Iceborne Community Edition. Join us at https://discord.gg/xPDVbhZgFJ to follow the development of this mod!

Iceborne Community Edition (ICE) is an overhaul mod for MHW: Iceborne, driven by community feedback and suggestions. ICE preserves the spirit of the game's core design and direction, but offers improvements to the game in an effort to provide a more balanced and diverse experience for all hunters.

This mod is a work-in-progress, and still in developement. 

ICE is compatible with online play. ICE hunters are matched exclusively with other ICE hunters to prevent negatively affecting vanilla hunters.

Features:
- Smoother Progression: Play through at your own pace, without being held back by cutscenes or unreasonable grinds.
- Quality-of-Life Additions: Spend more time enjoying each hunt, and less time in menus or stuck in base.
- Clutch Claw Rework: Let the Clutch Claw take a backseat, as you re-experience the fast-paced combat of MHW as it was originally intended. 
- Weapon Moveset Reworks: Master the 14 weapon types in new ways, with increased depth and variety in optimal combos for hunters.
- Skill Reworks: Make more impactful choices when it comes to skill loadouts. More variety, more active skills, less passives.
- Bug Fixes: Play the game with less pesky bugs to hold you back.

- - - -

# Table of Contents #

- [ICE Manager](#ice-manager)
- [Legacy - Installation Guide](#installation-guide)
- [Legacy - Save File System](#save-file-system)
- [Known Issues](#known-issues)
- [Change Log](#change-log)
  - [General Changes](#general-changes)
  - [Weapon Changes (Stable Build)](#weapon-changes-stable-build)
  - [Weapon Changes (Experimental Build)](#weapon-changes-experimental-build)

- - - -

# ICE Manager #
As of the latest release. ICE now has a version manager. It can be found here: <https://github.com/AsteriskAmpersand/Ice-Experimental/releases>.

The ICE Manager simplifies the ICE install and update process. As well as transferring save files and mods on your first install.

![](https://cdn.discordapp.com/attachments/920464605367644200/985342975871680602/unknown.png)

- You can first pick whichever version of ICE you prefer (the manager allows switching versions with one click). 
- You can transfer your base game save file and mods to ICE (mods may not all be compatible, the game will tell you of this when first booting up). 
- You can also update from now on, simply by clicking the "Update" button.
- You can Disable and Enable ICE with a single click as well
- You can fully uninstall ICE if you so desire.



# Installation Guide #

This instructions are no longer necessary, simply grabbing the [ICE Manager](#ice-manager) should be all that you need to install ICE.

## First Time Installation ##
Follow these steps if you've never installed ICE before:
1. Install Stracker's Loader and all it's prerequisites found here: <https://www.nexusmods.com/monsterhunterworld/mods/1982/>
2. On this Github page, click on the green "Code" button and then "Download ZIP".
3. Extract the contents of the ZIP file to a temporary location (Desktop, Downloads, etc).
4. Copy all the contents within the "ice-stable-main" (or "ice-experimental-main") folder directly to your root Monster Hunter World install folder (default path is `...\Steam\steamapps\common\Monster Hunter World\`. You have the right folder if "MonsterHunterWorld.exe" exists in that folder).
5. When asked about file conflicts, overwrite any existing files.
6. (Optional) Install any mods you want to use with ICE in the `...\Monster Hunter World\ICE\ntPC\` folder. Install any plugins in `...\Monster Hunter World\ICE\ntPC\plugins\`.
7. Launch game in Admin Mode (required only on first time installs). 
8. Check save file management section when you are asked to create a new ICE save file when launching the game.

## Updating Or Re-installing ICE ##
Follow these steps if you want to grab the latest version of ICE:
1. Click on the green "Code" button and then "Download ZIP".
2. Extract the contents of the ZIP directly to your root Monster Hunter World install folder (where MonsterHunterWorld.exe is located).
3. When asked about file conflicts, overwrite any existing files.

## Turning ICE ON / OFF ##
ICE supports easy on/off in case you want to switch back and forth between mods.
- If you want to disable ICE: Rename the main ICE folder to anything else.
- If you want to re-enable ICE: Rename the main ICE folder back to "ICE"
- If you want to reinstall ICE just download from repo and unzip into MHW.exe folder

## Uninstallation ##
If you want to uninstall ICE:
- (Easy Version) In the Monster Hunter World folder, delete the main ICE folder.
- (Full Version) In the Monster Hunter World folder, delete the main ICE folder, cryptbase.dll, loader.dll, ice_managed_code.dll. Then reinstall Stracker's Loader if you need it for other mods: <https://www.nexusmods.com/monsterhunterworld/mods/1982/>

## Installing Other Mods with ICE ##
If you want to install mods alongside ICE, we strongly recommend hunters stick with cosmetic/visual mods only. Gameplay mods will likely cause conflicts and compatibility issues. If you do wish to try gameplay mods at your own risk, we ask you to be considerate of other hunters and play offline only, just like you would without ICE.
1. Install mods in the `...\Monster Hunter World\ICE\ntPC\` folder. This ntPC folder is used instead of nativePC, while ICE is enabled.
2. Similarly, plugins are installed in the `...\Monster Hunter World\ICE\ntPC\plugins\` folder.
While ICE is enabled, mods and plugins are only loaded from the above folders. This allows you to manage your mods for ICE separately.

## Migrating from old ICE ##
If you were trying ICE before we switched to GitHub downloads, follow these one-time steps to update your ICE install:
1. Delete your old nativePC folder meant for ICE (save any mods you still want though, if you don't have a copy elsewhere).
2. On this Github page, click on the green "Code" button and then "Download ZIP".
3. Extract the contents of the ZIP file to a temporary location (Desktop, Downloads, etc).
4. Copy all the contents within the "ice-stable-main" (or "ice-experimental-main") folder directly to your root Monster Hunter World install folder (default path is `...\Steam\steamapps\common\Monster Hunter World\`. You have the right folder if "MonsterHunterWorld.exe" exists in that folder).
5. When asked about file conflicts, overwrite any existing files.
6. (Optional) Install any mods you want to use with ICE in the `...\Monster Hunter World\ICE\ntPC\` folder. Install any plugins in `...\Monster Hunter World\ICE\ntPC\plugins\`.
7. Launch game in Admin Mode (required only on first time installs)
8. Check save file management section when you are asked to create a new save file when launching the game.

- - - -

# Save File System #
This instructions are no longer necessary, simply grabbing the [ICE Manager](#ice-manager) should be all that you need to transfer your save file. First install ICE through the manager (on your preferred version), and then simply click Transfer Save.

ICE manages your character data in a separate save file named "SAVEDATA_ICE". The game normally uses the file named "SAVEDATA1000". These are both located in the standard save folder found at: `...\Steam\userdata\<steamId>\582010\remote\`

Because ICE incorporates changes that are not backwards compatible with the base game, it is necessary for us to separate your save data in this way. This system also allows hunters to quickly switch between ICE and vanilla freely without having to swap out save files. If enabled, ICE will automatically use the "SAVEDATA_ICE" save file. Otherwise, your game will continue to use the "SAVEDATA1000" save file as normal.

As always, it is recommended to make backups of your saves. It only takes one mistake to lose all your save data.

## Creating Your ICE Save File ##
If you boot up the game with ICE enabled for the first time and it says no save data detected, but you want to use your existing character data, then just follow these steps:
1. Hit yes to create a new ICE save but DON'T select a language.
2. If you want to start a new save file, then continue with the setup process in-game and skip the rest of the steps. Otherwise, continue with step 3.
3. Close the game after the game creates the save file but before selecting a language.
4. Navigate to your save folder at `...\Steam\userdata\<steamid>\582010\remote\`.
5. Delete the "SAVEDATA_ICE" file that's in that folder.
6. Make a copy of your "SAVEDATA1000" file and rename that copy to "SAVEDATA_ICE"
7. Start the game again.

## Updating Your ICE Save File ##
If you've continued to play on your vanilla save and want to overwrite your ICE save progress, then follow these steps:
1. Remove "SAVEDATA_ICE" if it exists (or throw it into another folder for safe keeping).
2. Make a new copy of "SAVEDATA1000".
3. Rename that copy to "SAVEDATA_ICE".

## Photo Data ##
ICE currently does not isolate photo/image data. As such, if you do use the in-game photo feature, make sure to backup the 3 photo data files in your save folder at `...\Steam\userdata\<steamid>\582010\remote\`. If the game detects a mismatch between your save file and your photo data, it will ask to create a new one, which would delete your photo data in the process.

- - - -

# Known Issues #

## Language Support ##
ICE currently only officially supports English language for text. You can use any voice language you prefer though.

## Incorrect Text / Descriptions ##
Much of the text found in ICE has not yet been updated to reflect changes made to the game. Our primary focus is on testing gameplay changes first, in an effort to avoid losing time and effort to keep descriptions up-to-date as we try different changes. Once we're further in development, we'll put more effort into covering changes we've made, and also updating descriptions from the game that are inaccurate or ambigious.

## Photo Data ##
ICE currently does not isolate photo/image data. As such, if you do use the in-game photo feature, make sure to backup the 3 photo data files in your save folder at `...\Steam\userdata\<steamid>\582010\remote\`. If the game detects a mismatch between your save file and your photo data, it will ask to create a new one, which would delete your photo data in the process.

- - - -

# Change Log #

## General Changes ##

### ──────────【 Multiplayer / Matchmaking 】────────── ###
While ICE is installed and enabled, hunters will only be matched with other ICE hunters. This is true when using matchmaking to find sessions or when creating/joining SOS. This is done for compatibility reasons and also out of courtesy to non-ICE hunters, so that non-ICE lobbies are not negatively impacted by any changes or differences in gameplay. Unlike other gameplay altering mods, hunters can freely play online with ICE.

### ──────────【 Monster Hitzones / Softening 】────────── ###
The dominance of the Clutch Claw has been drastically reduced to bring back the original combat pacing from base World. The goal is for softening to be a competitive option, but not a requirement.
- Softening effect on monster HZV has been reduced to `HZV+5` (down from `0.75*HZV + 25`).
- Monster "Clagger" behavior has been removed. Instead monsters will flinch, trip, and topple like they used to, before Iceborne.

Since Capcom reduced Monster hitzone values (HZV) to accommodate the powerful effects of softening, Monster hitzone values have been rebalanced in ICE to compensate for the Clutch Claw nerfs above. 
Details can be found here: https://docs.google.com/spreadsheets/d/1nzN2zYD1VbeEuKGlrYPRDZPHjfyy0y-SawwSEaTZ8OQ/edit?usp=sharing

AT Velkhana's unique HZV mechanic has also been slightly modified to account for these changes:
- Shot HZV Multipliers increased to 1.1/1.0/0.9 (up from 1.0/0.8/0.6)
These multipliers ensure that the head hitzone still counts towards WEX zones for gunners under the following conditions:
- Any time during aura Lv1
- Any time during aura Lv2
- Tenderized or broken head during aura Lv3
These values follow the assumed original developer intent, as they are below tenderized values in the vanilla tenderization formula and below melee multipliers values.

### ──────────【 Player 】────────── ###
- Attack cap increased to 3.0x (up from 2.0x). This reverts a nerf from IB.
- Element cap increased to 3.0x/+30 (up from 1.6x/+15).
- Status cap increased to 3.0x (up from 1.6x)
- Clutch Claw weapon attacks:
  - All weapons can now soften with a single use, as if they are heavy weapons.
  - Most weapons can now generate slinger ammo, as if they are light weapons.
  - Clutch Claw Boost skill (Shaver Decoration) no longer has any effect for now.

### ──────────【 Progression 】────────── ###

#### 【 Master Rank 】 ####
Master Rank experience gain has been doubled between MR25 and MR100 to help reduce the long grind that is required to unlock augments and play with other players in their Guiding Lands. While this grind may have served a purpose early on in Iceborne, the existence of DLC content that can be accessed immediately at low MR makes this grind awkward and out of place.

#### 【 Guiding Lands 】 ####
The Guiding Lands total zone experience cap mechanic has been disabled. Normally, a hunter would have to complete around 7100+ hunts in Lv7 GL zones in order to level all their zones to 7. While this did add a long term goal and encouraged multiplayer sessions for sharing GL zones, we find this unnecessary as:
1. The requirement was far too extreme for the vast majority of players to ever make a real dent in, let alone fully complete.
2. The Iceborne multiplayer community is naturally diminishing over time.

#### 【 Guaranteed Decorations 】 ####
Certain Decorations are now guaranteed to drop at least once during game progression. These were added for decorations that are particularly game changing and considered mandatory for certain weapons or playstyles.
<https://cdn.discordapp.com/attachments/920464605367644200/1001848843232620625/unknown.png>

#### 【 Decoration Drop Rates 】 ####
Decoration drop rates have been completely reworked and drastically improved.
- Decorations are classified by their value, which is based on the strength and usability of skills provided.
- Higher value decorations will drop from higher rarity Feystones. 
- Full details can be found here: <https://www.nexusmods.com/monsterhunterworld/mods/2162>

#### 【 Dracolites 】 ####
Dracolites have been added to Guiding Lands drop tables, providing hunters the option to continue upgrading their Safi'Jiiva weapons outside of the siege should either the siege not be available, or because they want some more variety in their hunts.

#### 【 Guiding Lands Materials 】 ####
- Guiding Lands Material mining and gathering rates have been strongly boosted.
- Full details can be found here: <https://www.nexusmods.com/monsterhunterworld/mods/2164>

#### 【 High Rank Augments 】 ####
Smithy costs for the following have been adjusted to better balance material usage in High Rank, and allow Rarity 6 weapons to act as a stronger progression step before Rarity 7 or 8 augmented weapons.
- Augments for Rarity 6 weapons changed to use 1x Streamstone instead of 1x Warrior's Streamstone.
- Augments for Rarity 7 weapons changed to use 1x Warrior's Streamstone (down from 2x Warrior's Streamstones).

The following new melding recipes have been added at the Elder Melder, to give hunters more control over their experience around farming High Rank augments:
- All 7 types of Warrior's Streamstones can be melded from 2 Warrior's Streamstones of any type.
- All 7 types of Hero's Streamstones can be melded from 2 Hero's Streamstones of any type.
- 2 Warrior's Streamstones can be melded from a single Hero's Streamstone of the same type.
- Hero's Streamstones can be melded from 4 Warrior's Streamstones of the same type.

### ──────────【 Skills 】────────── ###
While a more comprehensive rework and rebalancing of skills is planned for ICE in the future, some skills have been tweaked in the mean time with the an emphasis on increasing the variety of competitive options for hunters. This is mainly accomplished by:
1. Changing skills to have a more meaningful impact on gameplay.
2. Increasing the value of skills at lower levels.
> Weapon-specific interactions with certain skills will be covered in each weapon's section instead of here.

#### 【 General Changes 】 ####
- Coalescence:
  - Attack bonus changed to 12/18/24 (up from 12/15/18).
- Flinch Free:
  - "Brace Jewel 3" decoration size decreased to Lv1 (from Lv3).
  - Now affects airborne launches from other hunters. Lv2 will reduce the effect to a normal trip. Lv3 will negate the launches entirely. (See "Airborne Launches" under "Quality of Life" section for more details)
- Focus:
  - Bonus gauge generation increased to 10/18/25% (up from 5/10/20%).
  - > This change helps gauge-based weapons reach certain meaningful breakpoints.
- Fortify:
  - Duration increased to 9.1 hours (up from 50 minutes). 
  - > This partially reverts a nerf from IB, as Capcom's nerf only encouraged players to restart their Guiding Lands session every 50 minutes, rather than addressing any balance issues with Fortify.
- Heroics: Base Attack bonus changed from 0/5/5/10/15/25/40% to 5/10/15/20/25/30/40%.
- Item Prolonger:
  - Increased bonus to 33%/66%/100% (from 10%/25%/50%).
- Maximum Might:
  - Level 5 Affinity bonus increased to 50% (up from 40%).
  - Max Stamina time requirement decreased to 0 seconds (down from 5).
  - Lingering buff duration changed to only apply at level 4 (2 seconds) and level 5 (3 seconds).
- Non-Elemental Boost:
  - Base Attack bonus increased to 10% (up from 5%).
  - > This reverts a nerf from IB.
- Power Prolonger: 
  - Dual Blades & Switch Axe bonus decreased to 1.15x/1.30x/1.40x (down from 1.3x/1.6x/2.0x).
  - Long Sword, Charge Blade, & Insect Glaive bonus changed to 1.15x/1.30x/1.40x (was 1.1x/1.2x/1.4x).
- Quick Sheathe:
  - Speed bonus changed to 15/30/40% (from 10/20/40%).
- Weakness Exploit:
  - Affinity bonus changed to 15/30/50%. Softening requirement removed. 
  - > This reverts a nerf from IB and is intended to reduce reliance on Clutch Claw softening.

- Critical Element / True Critical Element (Set Bonus Skill):
  - Great Sword multipliers decreased to 1.35x/1.55x (down from 1.5x/1.7x).
  - Hunting Horn multipliers decreased to 1.35x/1.55x (down from 1.5x/1.7x).
- Critical Status / True Critical Status (Set Bonus Skill):
  - Great Sword multipliers decreased to 1.2x/1.4x (down from 1.4x/1.6x).
  - Hunting Horn multipliers decreased to 1.2x/1.4x (down from 1.4x/1.6x).
- Element Conversion (Set Bonus Skill):
  - Conversion rate increased to 8x for all weapons (up from 5x, or 2x for Bowguns).
  > This change brings the power level of the Alatreon set close to other element-based sets, allowing it to be used as a competitive alternative.
- Master's Touch (Set Bonus Skill):
  - Changed from triggering on critical hits to triggering on hitting weak spots.

### ──────────【 Equipment 】────────── ###

#### 【 Element/Status Balancing 】 ####
Some weapon types have been rebalanced to increase the variety in competitive equipment options for hunters to choose from. The following lists show what the rebalancing goals are for those weapon types. Some weapons will be able to better take advantage of at least the element/status available on their weapon. For these weapons, raw will still be competitive and be the most consistent option when not planning for specific match ups. Other weapons may now be able to run full element builds for certain playstyles.

#### 【 Armor Changes 】 ####
While a more comprehensive rework and rebalancing of armors is planned for ICE to increase the variety in build options for hunters that have meaningful impact on gameplay (with effects like Frostcraft from Velkhana), some specific sets have been adjusted in the mean time to preserve the limited options the game already did offer.

> Dev Comment: We understand these changes result in a decrease in the endgame power of hunters. While these endgame sets served as a nice final reward from Capcom for "finishing" the game, we don't think the power creep introduced by these sets are healthy in the context of ICE where we will be continually adding to the game. If/when we get around to incorporating additional endgame content, we may come back to revisit these changes when it's appropriate to have gear at these power levels.

- Fatalis and Velkhana Gamma Sets have been reduced in skills and deco slots. Fatalis Set no longer has access to Transcendence.
- These sets should still be competitive compared to options before their introduction.
- Changes to armors will be tracked separately on the Armor Spreadsheet.

#### 【 Weapon Changes 】 ####
Fatalis Weapons have been normalized (with the exception of LBG) to be 340 Raw, -30% affinity.

While weapons are normally dealt with on a more specific basis, this is a cross weapon nerf that was necessary both because of the inconsistencies it generates with weapon progressions as well as the aberrant stat values it had in specific outliers. This is a nerf that is still under evaluation but it will happen in one shape or another.

#### 【 General Changes 】 ####
- Health Regen augment:
  - For melee weapons, cooldown between procs decreased to 0.00s (down from 0.2s).
  - For ranged weapons, cooldown between procs decreased to 0.125s (down from 0.2s).
  - > The above changes were made to avoid inconsistent healing rates as result of movesets, weapon mechanics, and the engine's inability to correctly handle variable frame rates. Healing on ranged weapons will be virtually unchanged compared to intended rates from vanilla.
- Awakened Abilities:
  - Attack V: Attack bonus for GS and Hammer increased to 10 (up from 9), to match other weapons.
  - Attack VI: Attack bonus for GS and Hammer increased to 15 (up from 14), to match other weapons.
- Ammo tables for Safi LBGs have been updated to match Aquashot, but for other elements.

### ──────────【 Quality of Life 】────────── ###

#### 【 User Interface Changes 】 ####
- Equipment UIs now show true Attack (aka Raw) and true Element Damage/Buildup values for weapons.
  - > This removes the useless bloat multipliers that were artificially inflating numbers in UIs, but weren't actually being used by the game for any calculations.
- Chat UI:
  - Maximum message length increased to 60 (up from 40).
  - The selected chat channel no longer changes during certain actions (joining party/session/etc).
- Quantity selection UIs now support two new behaviors when increment/decrementing by 1:
  - Decrementing below 1 will now loop around to the maximum possible quantity.
  - Incrementing above the maximum possible quantity will now loop around to 1.
  - > These changes allow faster buying, selling, or melding of full stacks of items.

#### 【 Systems Changes 】 ####
- Despawn time for item drops from Monsters increased to 30 minutes (up from 1 or 2 minutes).
  - > This was done to help avoid situations where a hunter has to choose between interrupting their epic fight or forfeiting their rightfully earned loot. This wasn't a very interesting decision, in our opinion.
- Cutscenes:
  - A cutscene skip option has been enabled on most cutscenes in the game. Given most players will be experiencing ICE as a second (or later) playthrough, this QoL improvement should help shorten the time required to complete main story quests across all ranks.
  - > This is still a work-in-progress feature. Some cutscene audio might not skip correctly due to not being defined by the game as cutscene audio.
- Quest End Timer:
  - The timer for returning to base can now be skipped by holding the "Cancel Animation" input for 2 seconds ("Options" on PS, "Menu" on XB, X on PC).
- Astera Lift System:
  - Hunters can now utilize the lift system from the entrance of Astera, where they generally arrive after quests or expeditions (in front of the Resource Center).
  - When traveling to the "Tradeyard" using the lift system, the hunter will now arrive in the center of the Tradeyard.
  - > These changes are intended to decrease the amount of downtime that would otherwise be required to navigate around Astera, allowing hunters to spend more time hunting and less time walking.
- Botanical Research Center:
  - Fertilizer usage limit per quest removed (was 1 per quest).
  - Fertilizer maximum stackable duration increased to 20 quests (up from 9).
  - > Theses changes remove the constant attention required to maintain the Botanical Research Center. Hunters will only have to check on their BRC to reapply fertilizers as often as they need to collect their harvests (about every 15 to 20 quests once fully upgraded). These changes also make it so that restarting fertilizers (if expired) isn't a significant hassle.
  - Fertilizer balancing:
    - Research Point costs for Mega Fertilizer, Choice Mushroom Substrate, Thick Summoner Jelly, and Ancient Catalyst have been reduced. 
    - Ancient Catalyst duration increased to 5 quests (up from 4), to justify its higher cost relative to normal Catalyst.
    - > Since these fertilizers have lost their main advantage of allowing hunters to stack fertilzers faster between quests, they are now positioned as slightly more efficient versions of the basic fertilizers.
- Elder Melder:
  - Seasonal event tickets can be melded from 2 similar event tickets (down from 3).
  - Melding recipes for Whetfish Fin and Whetfish Fin+ have been added. The plus variant is unlocked in MR.

#### 【 Combat Changes 】 ####
- Mantle Expiration:
  - When a mantle expires, it will now automatically be unequipped without any interaction from the hunter.
- Airborne Launches:
  - Hunters can now protect themselves from being launched airborne by other hunters, using any of the available options that would protect against being knocked onto their butts. For example, Flinch Free Lv2 will reduce the launch to a trip, and Flinch Free Lv3 will negate the launch entirely.
  - Monster attacks are unaffected by this change.
- Guarding with Shield Weapons:
  - Guarding behavior changed to ignore attacks from other hunters.
  - Hunters will still see a hit effect (sparks), but the guarding hunter no longer consumes stamina and does not get locked into any follow-up guard reaction animations.
  - This change does not affect how hunters react to attacks they cannot block (attacks from behind, unblockable attacks, etc).
  - > In vanilla, shield weapons experienced extra downsides compared to other weapons when fighting in close proximity with other hunters. In particular, Lance hunters could have their Counter Thrusts triggered early by another hunter, resulting in getting hit by the Monster attack that they were preparing to counter. With this change, these potentially frustrating situations are removed from the game.
  
### ──────────【 Bug Fixes 】────────── ###

- DPS Tick Fix: The engine components responsible for specifically handling ticking damage effects have been upgraded to mitigate the negative effects of frame rate on player damage output. In some cases, player damage could be reduced as much as 25% just for not playing at a stable 60fps. Some examples here: <https://bit.ly/MHWEffectsOfFPS>
- Corrected some attacks that were incorrectly gaining extra hits at lower frame rates.
- Moonshots Fix: Aim behavior has been adjusted for Bow and Bowgun at short ranges to mitigate the occurrence of projectiles that incorrectly fly straight up (seemingly towards the moon/sky) and completely miss the intended target. This is sometimes refered to as "moonshots" by the community. An example can be seen here around the midpoint of the clip: <https://twitter.com/Irh_umbreon/status/1409001644411408391>
- Other weapon-specific bug fixes will be covered in each weapon's section instead of here.

### ──────────【 Monster Changes 】────────── ###

#### ──────────【 Monster Hitzones / Softening 】────────── ####
Details for this section are covered under General Changes near the top of this Change Log.

#### ──────────【 Alatreon 】────────── ####
Due to element damage output increasing significantly on many weapon types, Alatreon's weapon-specific element topple multipliers have been adjusted. A lower multiplier means a weapon's element damage will count for less and the hunter will need to deal more total element damage to reach each topple.
- Great Sword modifier decreased to 0.8x (down from 1.1x).
- Hunting Horn modifier decreased to 0.8x (down from 1.0x).
- Gunlance modifier decreased to 1.0x (down from 1.1x).



## Weapon Changes (Experimental Build) ##

### ──────────【 Equipment/Skill Changes 】────────── ###

- Health Regen Augment:
  - High Rank effect bonus decreased to 7%/11%/15% (down from 10%/15%/20%)
  - Master Rank effect bonus changed to 5%/8%/11%/14% (was 7.5%/9%/11%/14%)

### ──────────【 Dual Blades 】────────── ###

#### 【 Demon Mode & Archdemon Mode 】 ####
Demon Gauge generation and consumption has been reworked in an effort to make the management of Demon vs Archdemon Mode into a more impactful component of Dual Blades gameplay. These changes should provide hunters more options for combos as they flow back and forth between the two modes. Demon Mode will continue to be the primary method of dealing high damage at the cost of stamina, while Archdemon Mode will offer supplemental damage while stamina regenerates.

- Demon Mode:
	- Stamina consumption increased to 10/s (up from 5/s).
	- Demon Gauge generation has been reduced overall.
		- Most attacks generate 2.5% per hit (same as the original baseline for most attacks).
		- Heavier hitting attacks generate 5.0% per hit (down from as high as 20% per hit).
		- > This mainly addresses specific moves that were disproportionately generating far more Demon Gauge than other moves, and trivializing gauge generation.
	- Automatically de-activates if the hunter is sent flying by an attack.
	- Turning Demon Mode Off:
		- When performed after an attack, now has an active hitbox with the following stats:
			- 8+8 MV
			- 0.6x+0.6x Element and Status Modifier
		- Can be performed sooner after Blade Dance.
		- > These changes allow Demon Mode attacks to flow directly into Archdemon Mode attacks.

- Archdemon Mode:
	- Enables the use of Demon Mode Dashes.
		- Each dash will consume 5% Demon Gauge while not in Demon Mode.
		- > Known Issue: These dashes do not have a proper animation for handling weapon grip style (standard vs reverse). This will be fixed in a future update.
	- Rising Slash uses Demon Mode versions with higher MV.
	- Left/Right Roundslash:
		- Consumes 5% Demon Gauge while not in Demon Mode.
		- Damage greatly enhanced (see General Changes section).
	- Demon Flurry:
		- MV increased to 12+12+9+9+9+22+22 (up from 9+9+7+7+3+17+17).
		- Element and Status Modifier increased to 0.8x+0.8x+0.6x+0.6x+0.6x+1.5x+1.5x (up from 0.8x+0.8x+0.8x+1.0x+1.0x+1.0x).
		- Now combos into Demon Flurry Rush.
		- > This buff properly sets up Demon Flurry as a strong attack worth spending Demon Gauge on during Archdemon Mode, without overshadowing Demon Mode.

#### 【 Status Buildup Modifiers 】 ####
Each attack's Status Modifier has been increased to match their Element Modifier. To understand the reasoning for this change, it is best to cover the history of these modifiers.
- During MHW, Dual Blades had a 1.0x modifier for both Element and Status on every attack. This was generally the case for most weapons, and still is even in Iceborne.
- With the launch of Iceborne (v10.10), Capcom was concerned about the power level of element-based builds, and some weapons received overly massive nerfs to their Element and Status Modifiers. For Dual Blades, they nerfed both modifiers by 20% to 60% depending on the attack (with Status being nerfed either the same or slightly more than Element).
- With the Stygian/Safi Update (v12.01), Capcom partially reverted the nerfs. Depending on the attack, some Element Modifiers nerfs were fully reverted or were reduced to only 40% compared to MHW. Some Status Modifiers were very slightly increased, but the majority were untouched.

While Iceborne did receive some significant increases in element-based build power (examples include additional Element Up skill levels, buffs to Critical Element multipliers, massive element multiplier on Purple Sharpness), the same cannot be said of status-based builds. As such, it is likely Capcom simply overlooked these Status Modifiers when they decided to go back and partially revert the Element Modifier nerfs.

#### 【 General Changes 】 ####
Most following changes are targeted at increasing the variety of combos and options available to hunters:

- Left/Right Fade Slash:
	- MV increased to 11+11 (up from 7).
	- Element and Status Modifier increased to 0.75x+0.75x (was 0.8x).
	- > This move found very little use in vanilla with such low damage and minor repositioning value. With this change, both Fade Slashes can be used to situationally loop and extend the Demon Slash combo, during windows of opportunity that are too short for stronger/longer follow-up attacks.
- Rising Slash (Demon Mode):
	- MV increased to 12 (up from 9).
	- > Rising Slash bridges many different moves, but was too heavily dragging down the efficacy of any combo that included it.
- Left/Right Roundslash:
	- MV increased to 19+11+7 (up from 15+7+5).
	- Element and Status Modifier increased to 0.8x+0.8x+0.8x (up from 0.6x+0.6x+0.6x).
	- > While the damage on these attacks may have seemed reasonable per hit, the damage was too low relative to animation length for a Demon Mode attack.
- Left/Right Double Roundslash:
	- MV increased to 27+15+12 (up from 19+11+7).
	- > While the damage on these attacks may have seemed reasonable per hit, the damage was too low relative to animation length for a Demon Mode attack.
- Special Claw Attack:
	- Claw Attack:
		- Can be performed outside of Demon Mode, if Archdemon Mode is active. Consumes 20% Demon Gauge if used in this way.
		- Can be performed after Left/Right Roundslash (L2 on PS, LT on XB).
		- Can be performed after Blade Dance (L2 on PS, LT on XB).
		- Can be performed after Demon Flurry (L2 on PS, LT on XB).
		- > Using a directional input in addition to the input indicated above, will instead result in performing an Evade Shot.
	- Spinning Rising Slash:
		- Element and Status Modifier increased to 1.25x+1.25x+1.25x+1.25x (up from 1.0x+1.0x+1.0x+1.0x).
	- > These changes allow Spinning Rising Slash to be used as a combo finisher, and makes up for the loss of Monster Clagger in ICE.


### ──────────【 Hammer 】────────── ###

#### 【 Power Charge Dash Addition 】 ####
- Power Charge when you are already in Power Charge State instead starts a dash which removes Power Charge State and instead sets the Charge Level to 3. This move is treated as part of a Charge and can combo into any Charge follow-up or continued into a Charge.
	
#### 【 Combo Continuation 】 ####
The following combo continuation is intoduced and is inteded to be a possible continuation of the above listed addition of the Power Charge Dash.
- Spinning Bludgeon into Spinning Strong Upswing can now combo into Big Bang IV
- By Releasing R without Directional Input it combos into [Half] Brutal Big Bang
- By Releasing R with Directional Input it combos into Spinning Bludgeon
- By Holding R through it, it leads back into Charging.
- The Dash has 30 frames of Hyperarmor (Frame 10 to Frame 40)
