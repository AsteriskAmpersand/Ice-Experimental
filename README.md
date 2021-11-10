# Iceborne Community Edition #

Welcome to the download page for Iceborne Community Edition. Join us at https://discord.gg/xPDVbhZgFJ to follow the development of this mod!

Iceborne Community Edition is a holistic rework of MHW: Iceborne. We attempt to address multiple major gripes a significant section of the playerbase had with an otherwise great game. The goal of ICE is to preserve the spirit of the game's core design, but improve on its limitations and flaws to provide a more enjoyable experience that can still be recognized as Monster Hunter gameplay.

- - - -

# Installation Guide #

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

## Quest: ★1 Learning the Clutch ##
This quest cannot currently be completed as intended due to the fact that Clagger is removed in ICE. A temporary fix has been put in place to allow the quest to be completed by killing the Great Jagras. In the future, we'll address this issue properly by updating the quest to account for Clagger removal, or replace the quest entirely.

- - - -

# Change Log #

## General Changes ##

### ──────────【 Multiplayer / Matchmaking 】────────── ###
While ICE is installed and enabled, hunters will only be matched with other ICE hunters. This is true when using matchmaking to find sessions or when creating/joining SOS. This is done for compatibility reasons and also out of courtesy to non-ICE hunters, so that non-ICE lobbies are not negatively impacted by any changes or differences in gameplay. Unlike other gameplay altering mods, hunters can freely play online with ICE.

### ──────────【 Monster 】────────── ###
The dominance of the Clutch Claw has been drastically reduced to bring back the original combat pacing from base World. The goal is for softening to be a competitive option, but not a requirement.
- Softening effect on monster HZV has been reduced to `HZV+5` (down from `0.75*HZV + 25`).
- Monster "Clagger" behavior has been removed. Instead monsters will flinch, trip, and topple like they used to, before Iceborne.

Since Capcom reduced Monster hitzone values to accommodate the powerful effects of softening, Monster  hitzone values have been rebalanced in ICE to compensate for the Clutch Claw nerfs above. 
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
<https://cdn.discordapp.com/attachments/879277879987408977/880205529086066748/unknown.png>

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

### ──────────【 Skills 】────────── ###
While a more comprehensive rework and rebalancing of skills is planned for ICE in the future, some skills have been tweaked in the mean time with the an emphasis on increasing the variety of competitive options for hunters. This is mainly accomplished by:
1. Changing skills to have a more meaningful impact on gameplay.
2. Increasing the value of skills at lower levels.
> Weapon-specific interactions with certain skills will be covered in that weapon's section instead of here.

#### 【 General Changes 】 ####
- Weakness Exploit:
  - Affinity bonus changed to 15/30/50%. Softening requirement removed. 
  - > This reverts a nerf from IB and is intended to reduce reliance on Clutch Claw softening.
- Focus:
  - Bonus gauge generation increased to 10/18/25% (up from 5/10/20%).
  - > This change helps gauge-based weapons reach certain meaningful breakpoints.
- Heroics: Base Attack bonus changed from 0/5/5/10/15/25/40% to 5/10/15/20/25/30/40%.
- Flinch Free:
  - "Brace" decoration size decreased to Lv1 (from Lv3).
  - Now affects airborne launches from other hunters. Lv2 will reduce the effect to a normal trip. Lv3 will negate the launches entirely. (See "Airborne Launches" under "Quality of Life" section for more details)
- Fortify:
  - Duration increased to 9.1 hours (up from 50 minutes). 
  - > This partially reverts a nerf from IB, as Capcom's nerf only encouraged players to restart their Guiding Lands session every 50 minutes, rather than addressing any balance issues with Fortify.
- Quick Sheathe:
  - Speed bonus changed to 15/30/40% (from 10/20/40%).
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
- Alatreon Divinity (Set Bonus):
  - Element Conversion rate for normal weapons increased to 8% (up from 5%).
  - Element Conversion rate for Bowguns increased to 8% (up from 2%).
  > The above changes allow the Alatreon set to perform closer to other element oriented sets.

### ──────────【 Equipment 】────────── ###

#### 【 Raw vs Element Balancing 】 ####
Some weapon types have been rebalanced to increase the variety in competitive equipment options for hunters to choose from. The following lists show what the rebalancing goals are for those weapon types. Some weapons will be able to better take advantage of at least the element/status available on their weapon. For these weapons, raw will still be competitive and be the most consistent option when not planning for specific match ups. Other weapons may now be able to run full element builds for certain playstyles.

Raw/Element Weapon + Raw Build:
- Long Sword
- Lance
- Insect Glaive

Element Weapon + Element Build:
- Great Sword (only for new alternative combo playstyle)

#### 【 Armor Changes 】 ####
While a more comprehensive rework and rebalancing of armors is planned for ICE to increase the variety in build options for hunters that have meaningful impact on gameplay (with effects like Frostcraft from Velkhana), some specific sets have been adjusted in the mean time to preserve the limited options the game already did offer.

> Dev Comment: We understand these changes result in a decrease in the endgame power of hunters. While these endgame sets served as a nice final reward from Capcom for "finishing" the game, we don't think the power creep introduced by these sets are healthy in the context of ICE where we will be continually adding to the game. If/when we get around to incorporating additional endgame content, we may come back to revisit these changes when it's appropriate to have gear at these power levels.

- Fatalis and Velkhana Gamma Sets have been reduced in skills and deco slots. Fatalis Set no longer has access to Transcendence.
- These sets should still be competitive compared to options before their introduction.
- Changes to armors will be tracked separately on the Armor Spreadsheet.

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
- Equipment UIs now show true Attack (aka Raw) and true Element values for weapons.
  - > This removes the useless bloat multipliers that aren't actually used by the game for any calculations.
- Chat channel no longer changes during certain actions (joining party/session/etc).

#### 【 Systems Changes 】 ####
- Despawn time for item drops from Monsters increased to 30 minutes (up from 1 or 2 minutes).
  - > This was done to help avoid situations where a hunter has to choose between interrupting their epic fight or forfeiting their rightfully earned loot. This wasn't a very interesting decision, in our opinion.
- Cutscene Skip option enabled on most cutscenes in the game. Given most players will be experiencing ICE as a second (or later) playthrough, this quality of life improvement should help shorten the time required to complete main story quests across all ranks.
  - > This is still a work-in-progress feature. Some cutscene audio might not skip correctly due to not being defined by the game as cutscene audio.
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

#### 【 Combat Changes 】 ####
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
- Moonshots Fix: Aim behavior has been adjusted for Bow and Bowgun at short ranges to mitigate the occurrence of projectiles that incorrectly fly straight up (seemingly towards the moon/sky) and completely miss the intended target. This is sometimes refered to as "moonshots" by the community. An example can be seen here around the midpoint of the clip: <https://twitter.com/Irh_umbreon/status/1409001644411408391>



## Weapon Changes (Experimental Build) ##

### ──────────【 Sword & Shield 】────────── ###

#### 【 New Parry Option 】 ####
The following changes are intended to give hunters an additional defensive option that fits the theme of the weapon (parrying with a buckler shield) while increasing variety in gameplay. Hunters that master this new technique will be able to weave counter-attacks against weaker Monster attacks into their existing play.
- Guard Slash:
	- Now has a guardpoint starting from 0.10s from the start of the animation, lasting 0.30s.
	- When hit during the guardpoint, small knockbacks will result in immediately counter-attacking with a Shield Bash. This Shield Bash can combo into Leaping Slash (Triangle) or directly into Perfect Rush (Circle).
	- > Hunters will need to recognize and react accordingly to which attacks they can and cannot "parry", as many Monster attacks will be too strong for a small shield. In addition, when comboing directly from Shield Bash into Perfect Rush, the Shield Bash will effectively replace the first hit in Perfect Rush I.

#### 【 Quality of Life Changes 】 ####
- Backstep (aka Backhop):
	- When performed after an unsheathed forward roll, hunters can now hold a desired direction and press Circle early to queue a directional Backstep.
		- > Previously, early inputs would result in comboing into a backwards Backstep and late inputs would result in comboing into other attacks, leaving only a small 0.250s window that was difficult for hunters to consistently hit. With this change, early inputs are no longer an issue.
	- When performed after starting to guard, the time available to input a Backstep safely has been increased to 0.417s (up from 0.283s).
		- > This increases the window that hunters have by 50%, which should greatly increase the reliability of using Backstep right after a guard.
- Slinger Aim vs Slinger Burst Aim Mode Toggle:
	- The hunter's current selected mode will now still be retained upon sheathing (previously was resetting to Slinger Aim Mode).

#### 【 General Changes 】 ####
Many of the following changes are targeted at one of the following goals:
- Increasing the variety of combos and options available to hunters. Less used slashing attacks can now be better combined with existing high damage slashes (Lateral Slash + Return Stroke) to create longer and stronger combos without needing to utilize the weaker Spiral Slash as often. In addition, shield attacks can be comfortably used in place of slashes, allowing hunters to trade only a small amount of damage for added Stun buildup.
- Reducing the dominance of Perfect Rush. The changes to Perfect Rush's damage help provide shorter combos (Slash combos, Shield combos, Falling Bash) a chance at competing in shorter windows of opportunities, while still maintaining Perfect Rush's advantage of dealing high damage for larger windows. In many situations, it can be better to use other options if the hunter does not have a large enough window to safely perform up to Perfect Rush II.

- Chop:
	- MV increased to 17 (up from 14).
- Side Slash:
	- MV increased to 14 (up from 13).
- Rising Slash:
	- MV increased to 15 (up from 14).
- Short Shield Bash:
	- MV increased to 15 (up from 6).
- Shield Attack:
	- MV increased to 20 (up from 8).
- Shield Bash:
	- MV increased to 20 (up from 16).
- Hard Bash:
	- MV increased to 36 (up from 31).
- Perfect Rush I:
	- MV decreased to 40+40+50 (down from 45+45+60).
- Perfect Rush II:
	- MV increased to 60 (up from 55).
- Clutch Claw Weapon Attack:
	- Final Hit:
		- Partbreak Modifier increased to 2.35x (up from 1.00x).
		- > Compensates for first three hits having a Partbreak Mod of 0.0x.

### ──────────【 Hammer 】────────── ###

#### 【 Power Charge Dash Addition 】 ####
- Power Charge when you are already in Power Charge State instead starts a dash which removes Power Charge State and instead sets the Charge Level to 3. This move is treated as part of a Charge and can combo into any Charge follow-up or continued into a Charge.
	
#### 【 Combo Continuation 】 ####
The following combo continuation is intoduced and is inteded to be a possible continuation of the above listed addition of the Power Charge Dash.
- Spinning Bludgeon into Spinning Strong Upswing can now combo into Big Bang IV

#### 【 Important 】 ####
- The current implementation is not Multiplayer safe. There is a high risk of visual glitching and desynchronization. Game stability is also dubious in Multiplayer.


### ──────────【 Lance 】────────── ###

#### 【 General Changes 】 ####
Lance has a solid playstyle and was only lacking damage to compete with other weapons. As such, most attacks were simply increased in power to an appropriate level relative to other weapons. In addition, the Raw vs Element balance was adjusted to increase the variety of competitive weapon options.

- Mid Thrusts:
  - MV increased to 23/23/30 (up from 20/20/27).
  - Element and Status Modifiers increased to 0.8x/0.8x/0.9x (up from 0.7x/0.7x/0.7x).
- High Thrusts:
  - MV increased to 25/25/30 (up from 22/22/27).
  - Element and Status Modifiers increased to 0.8x/0.8x/0.9x (up from 0.7x/0.7x/0.7x).
- Wide Sweeps:
  - MV increased to 32/32/40 (up from 20/20/20).
  - Element and Status Modifiers increased to 1.0x/1.0x/1.2x (up from 0.7x/0.7x/0.7x).
  - Changed to have Mind's Eye effect.
- Counter Thrust:
  - MV increased to 46 (up from 40).
  - Element and Status Modifiers increased to 1.25x (up from 0.7x).
- Power Guard:
	- When held for 1.2s, increases Counter Thrust damage by 1.5x and grants the effects of Guard Up (previously only granted the effects of Guard Up).
	- > This change is intended to give an alternative incentive for committing to a Power Guard, rather than solely for Guard Up. While this option is powerful, it is limited by OFG procs, stamina usage, increased chip damage, and high animation commitment. We understand that Power Guard should not creep too high as it is the safest guard option available, and are keeping an eye on how this new mechanic fares in all levels of Lance play before it moves to Stable.
- Leaping Thrust:
  - MV increased to 11 (up from 8).
  - Element and Status Modifiers increased to 0.4x (up from 0.3x).
- Dash Attack:
	- Startup time significantly reduced when used after Mid Thrust III, High Thrust III, or Wide Sweep III.
	- No longer cancels when running into walls or terrain.
  - MV increased to 12 (up from 11).
  - Element and Status Modifiers increased to 0.5x (up from 0.2x).
- Finishing Thrust:
  - MV increased to 60 (up from 50).
  - Element and Status Modifiers increased to 1.6x (up from 0.8x).
- Finishing Twin Thrust:
  - MV increased to 30+60 (up from 25+50).
  - Element and Status Modifiers increased to 0.8x+1.6x (up from 0.7x+0.8x). 
- Reverse Attack:
  - MV increased to 60 (up from 50).
  - Element and Status Modifiers increased to 1.6x (up from 0.8x).
- Jumping Thrust / Advancing Jump Thrust:
  - MV increased to 32 (up from 30).
  - Element and Status Modifiers increased to 1.0x (up from 0.7x).
- Dash Attack (Midair):
  - MV increased to 30 (up from 25).
  - Element and Status Modifiers increased to 1.0x (up from 0.7x).
- Shield Attack:
  - MV increased to 24 (up from 14).
  - Partbreak Modifier increased to 1.2x (up from 1.0x).
  - Stun buildup increased to 45 (up from 27).
  - Exhaust buildup increased to 30 (up from 27).
- Counter Claw (Second Hit):
  - MV increased to 24 (up from 16).
  - Stun buildup increased to 35 (up from 30).
  - Exhaust buildup decreased to 30 (down from 33).
- Mounting Finishing Thrust: 
  - MV increased to 40+20+80 (up from 40+10+20).
	- Element Modifiers changed to 1.0x+0.5x+2.0x (was 1.0x+1.0x+1.0x).
	- Status Modifiers changed to 1.0x+0.5x+2.0x (was 0.7x+0.7x+0.7x).
	- Third Hit:
		- Partbreak Modifier increased to 1.75x (up from 1.0x).
		- > Compensates for first two hits having a Partbreak Mod of 0.0x.
- Clutch Claw Weapon Attack:
  - Second Hit: 
    - Partbreak Modifier increased to 1.75x (up from 1.0x).
    - > Compensates for the first hit having a Partbreak Mod of 0.0x.
		