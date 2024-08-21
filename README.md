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

- [Setup Information](#ice-setup-information)
- [Change Log](#change-log)
  - [General Changes](#general-changes)
  - [Weapon Changes (Stable Build)](https://github.com/AsteriskAmpersand/Ice-Stable#weapon-changes-stable-build)
  - [Weapon Changes (Experimental Build)](https://github.com/AsteriskAmpersand/Ice-Experimental#experimental-weapon-changes)

- - - -

# Setup Information #
Information for the following topics can now be found on our GitHub Wiki here: <https://github.com/AsteriskAmpersand/Ice-Stable/wiki>
- Installing ICE
- Updating ICE
- Switching between ICE and vanilla
- Uninstalling ICE
- Managing ICE save data
- Known Issues

- - - -

# Change Log #

## General Changes ##

### ──────────【 Multiplayer / Matchmaking 】────────── ###
While ICE is installed and enabled, hunters will only be matched with other ICE hunters. This is true when using matchmaking to find sessions or when creating/joining SOS. This is done for compatibility reasons and also out of courtesy to non-ICE hunters, so that non-ICE lobbies are not negatively impacted by any changes or differences in gameplay. Unlike other gameplay altering mods, hunters can freely play online with ICE.

### ──────────【 Clutch Claw Rework 】────────── ###
The dominance of the Clutch Claw has been drastically reduced to bring back the original combat pacing from base World. The goal is for softening to be a strong optional tool for the Hunter to use as desired, rather than a required component in general play.
- Softening effect on monster HZV has been reduced to `HZV+5` (down from `0.75*HZV + 25`).
- Monster "Clagger" behavior has been removed. Instead monsters will flinch, trip, and topple like they used to, before Iceborne.
- Clutch Claw weapon attacks:
  - All weapons can now soften with a single use, as if they are heavy weapons.
  - Most weapons can now generate slinger ammo, as if they are light weapons.
  - Clutch Claw Boost skill (Shaver Decoration) no longer has any effect for now.

### ──────────【 Monster Hitzones 】────────── ###
Monster hitzone values (HZV) have been rebalanced in Master Rank to compensate for reduction in Clutch Claw power. All weapons have a primary weakzone to aim for, without the need for softening. Some secondary weakzones that previously required softening to active, are now either always weakzones or can still become weakzones through softening. Additionally, some monsters have had their existing element weakness amplified so that bringing element is more of an option.

Full details for individual monsters can be found on our HZV Rework spreadsheet: https://docs.google.com/spreadsheets/d/1nzN2zYD1VbeEuKGlrYPRDZPHjfyy0y-SawwSEaTZ8OQ/edit?usp=sharing

In addition, the following monsters received other changes that are worth calling out specifically.

- Alatreon:
  - Head & Neck: Shot HZV increased to 50 (up from 30).
  - Body: Shot HZV decreased to 30 (down from 45).
  - Arms: Shot HZV increased to 40 (up from 20).
  - Dragon HZV modifier:
    - Increased to 0.5x during Fire and Ice states (up from 0.1x).
    - Increased to 1.1x during Dragon state (up from 0.7x).
    - > These changes are intended to enable Dragon to be a 3rd alternative element pick for a wider range of weapon types.
- Behemoth:
  - Head: Blunt HZV increased to 65 (up from 55).
  - Arms: Blunt HZV increased to 45 (up from 40).
- Lavasioth:
  - "Broken" HZVs for Head, Body, Legs, and Tail increased to match "Heated" HZVs.
  - Various HZVs raised to prevent bouncing with White or Purple sharpness.
- Lunastra:
  - Head: Sever HZV increased to 45 (up from 40) for both HR and MR.
  - Body: Sever and Blunt HZV increased to 20 (up from 17) for MR.
  - Back: Sever and Blunt HZV increased to 20 (up from 17) for MR.
  - Hindlegs:
    - Sever HZV increased to 45 (up from 30) for both HR and MR.
    - Blunt HZV increased to 40 (up from 25) for both HR and MR.
    - > This change makes the hindlegs a proper secondary weakzone for Blademasters.
  - Wings:
    - Shot HZV increased to 45 (up from 40) for both HR and MR.
    - > This change makes the wings a proper secondary weakzone for Gunners.
- Kulve Taroth (MR):
  - All HZVs changed to match those found in HR.
- Namielle:
  - Sever, Blunt, and Shot HZVs increased while in Normal state.
  - Fire HZVs increased while in Dehydrated state.
  - > These changes partially reduce the drastic swings in weaknesses across the two states.
- Uragaan:
  - Forearms: Sever and Blunt HZV increased to 40 (up from 25 and 30).
- Velkhana:
  - Arch-Tempered HZV modifiers:
    - Shot HZV Multipliers increased to 1.1x/1.0x/0.9x (up from 1.0x/0.8x/0.6x)
    - These multipliers ensure that the head hitzone still counts towards WEX zones for gunners under the following conditions:
      - Any time during aura Lv1
      - Any time during aura Lv2
      - Tenderized or broken head during aura Lv3
    - > These values were chosen to follow what we assume to be Capcom's original intent. They are below tenderized values in the vanilla softening formula and below melee multipliers values.

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

New melding recipes have been added at the Elder Melder to allow hunters to trade Warrior's and Hero's Streamstones. See details for Elder Melder under [Quality of Life](https://github.com/AsteriskAmpersand/Ice-Stable#-quality-of-life-) for more details.

### ──────────【 Skills 】────────── ###
While a more comprehensive rework and rebalancing of skills is planned for ICE in the future, some skills have been tweaked in the mean time with the an emphasis on increasing the variety of competitive options for hunters. This is mainly accomplished by:
1. Changing skills to have a more meaningful impact on gameplay.
2. Increasing the value of skills at lower levels.
> Weapon-specific interactions with certain skills will be covered in each weapon's section instead of here.

#### 【 General Changes 】 ####
- Coalescence:
  - Attack bonus changed to 6/12/18 (was 12/15/18).
- Flinch Free:
  - "Brace Jewel 3" decoration size decreased to Lv1 (from Lv3).
  - Now affects airborne launches from other hunters. Lv2 will reduce the effect to a normal trip. Lv3 will negate the launches entirely. (See "Airborne Launches" under "Quality of Life" section for more details)
- Focus:
  - Bonus gauge generation increased to 10/18/25% (up from 5/10/20%).
  - > This change helps gauge-based weapons reach certain meaningful breakpoints.
- Fortify:
  - Duration increased to 9.1 hours (up from 50 minutes).
  - > This partially reverts a nerf from IB, as Capcom's nerf only encouraged players to restart their Guiding Lands session every 50 minutes, rather than addressing any balance issues with Fortify.
- Heroics:
  - Base Attack bonus changed from 0/5/5/10/15/25/40% to 5/10/15/20/25/30/40%.
- Item Prolonger:
  - Item duration bonus increased to 33%/66%/100% (from 10%/25%/50%).
- Maximum Might:
  - Affinity bonus changed to 10%/20%/30%/40%/50% (from 10%/20%/30%/40%/40%).
  - Max Stamina time requirement changed to 0/0/0/0/0s (from 5/5/5/5/0s).
  - Lingering buff duration changed to 0/0/0/1/2s (from 2/3/3/4/0s).
- Non-Elemental Boost:
  - Base Attack bonus increased to 10% (up from 5%).
  - > This reverts a nerf from IB.
- Offensive Gaurd:
  - Base Attack bonus increased to 6%/12%/20% (up from 5%/10%/15%).
- Power Prolonger:
  - Dual Blades & Switch Axe duration bonus decreased to 1.15x/1.30x/1.40x (down from 1.3x/1.6x/2.0x).
  - Long Sword, Charge Blade, & Insect Glaive duration bonus changed to 1.15x/1.30x/1.40x (was 1.1x/1.2x/1.4x).
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
- Dragonvein Awakening / True Dragonvein Awakening (Set Bonus Skill):
  - Element Limit Override increased to 3.5x/4.0x of Base Element (up from 2.2x/2.55x generally, up from 1.8x/2.35x for Bowguns).
  - Status Limit Override increased to 3.5x/4.0x of Base Status (up from 1.7x/2.0x).
- Element Conversion (Set Bonus Skill):
  - Conversion rate increased to 8x for all weapons (up from 5x, or 2x for Bowguns).
  > This change brings the power level of the Alatreon set close to other element sets, allowing it to be used as a competitive alternative.
- Master's Touch (Set Bonus Skill):
  - Activation condition changed to "on weakspot hits" (was "on Critical hits").

### ──────────【 Equipment 】────────── ###

#### 【 Element/Status Balancing 】 ####
Some weapon types have been rebalanced to increase the variety in competitive equipment options for hunters to choose from. Some weapons will be able to better take advantage of at least the element/status available on their weapon, despite optimizing for Attack overall. Other weapons may now be able to run full element builds for certain playstyles or specific matchups.

#### 【 Armor Changes 】 ####
While a more comprehensive rework and rebalancing of armors is planned for ICE to increase the variety in build options for hunters that have meaningful impact on gameplay (with effects like Frostcraft from Velkhana), some specific sets have been adjusted in the mean time to preserve the limited options the game already did offer.

> Dev Comment: We understand these changes result in a decrease in the endgame power of hunters. While these endgame sets served as a nice final reward from Capcom for "finishing" the game, we don't think the power creep introduced by these sets are healthy in the context of ICE where we will be continually adding to the game. If/when we get around to incorporating additional endgame content, we may come back to revisit these changes when it's appropriate to have gear at these power levels.

- Fatalis and Velkhana Gamma Sets have been reduced in skills and deco slots. Fatalis Set no longer has access to Transcendence.
- These sets should still be competitive compared to options before their introduction.
- Changes can be seen using Chantox's MHW Builder when selecting "ICE" mode: <https://mhw-builder.vercel.app/>

#### 【 Weapon Changes 】 ####
Safi'Jiiva Light Bowguns:
  - Ammo tables have been updated to match Aquashot, but for each of their respective element types.

Fatalis Rarity 12 Weapons (All, except for LBG):
  - Base Attack standardized to 340 Attack (was 340 to 370).
  - Base Affinity standardized to -30% (was -20% to -40%).
  - > This cross-weapon nerf was performed to address a number of issues introduced by these weapons such as unnecessarily shifting the meta away from element. We also understand some weapons likely were given higher stats (such as Lance) to compensate for their poor performance relative to other weapons. However, we believe improving these weapons' core movesets is a better solution than to only tack on a buff to Fatalis weapons.

#### 【 Augments and Upgrades 】 ####
- Health Regen augment:
  - Healing Effect:
    - High Rank effect decreased to 7%/11%/15% (down from 10%/15%/20%)
    - Master Rank effect changed to 5%/8%/11%/14% (was 7.5%/9%/11%/14%)
  - Cooldown:
    - For melee weapons, cooldown between procs decreased to 0.00s (down from 0.2s).
    - For ranged weapons, cooldown between procs decreased to 0.125s (down from 0.2s).
    - > The above changes were made to avoid inconsistent healing rates as result of movesets, weapon mechanics, and the engine's inability to correctly handle variable frame rates. Healing on ranged weapons will be virtually unchanged compared to intended rates from vanilla.
- Awakened Abilities:
  - Attack V: Attack bonus for Greatsword and Hammer increased to 10 (up from 9), to match other weapons.
  - Attack VI: Attack bonus for Greatsword and Hammer increased to 15 (up from 14), to match other weapons.

#### 【 Stat Limits 】 ####
- Attack Limit increased to 3.0x of Base Attack (up from 2.0x). This reverts a nerf from IB.
- Element Limit increased to 3.0x/+30 of Base Element (up from 1.6x/+15 generally, up from 1.57x/+15 for Bowguns).
- Status Limit increased to 3.0x of Base Status (up from 1.6x).
- Stun Buildup Limit increased to 3.0x of Base Stun Buildup (up from 2.0x).
- Exhaust Buildup Limit increased to 3.0x of Base Exhaust Buildup (up from 2.0x).
- Mount Buildup Limit increased to 3.0x of Base Mount Buildup (up from 2.0x).

### ──────────【 Quality of Life 】────────── ###

#### 【 User Interface Changes 】 ####
- Equipment UIs:
  - Attack values now show true Attack (was inflated by 1.2x to 5.2x depending on weapon).
  - Element Damage/Buildup values now show true Element Damage/Buildup (was inflated by 10x for all weapons).
  - > Player damage is unaffected. These changes only remove the various "bloat" multipliers that were causing misleading values to be displayed in the UI. Now players can see the true values being used by the game, which will correctly match values indicated in skill bonuses.
- Chat UI:
  - Maximum message length increased to 60 (up from 40).
  - The selected chat channel no longer changes during certain actions (joining party/session/etc).
- Quantity selection UIs now support two new behaviors when increment/decrementing by 1:
  - Decrementing below 1 will now loop around to the maximum possible quantity.
  - Incrementing above the maximum possible quantity will now loop around to 1.
  - > These changes allow faster buying, selling, or melding of full stacks of items.
- Many UIs have been made more responsive to inputs and interactions. Some examples are listed below.
  - Start Menu:
    - Intro and outro animations sped up.
    - Automatically skips the intro animation without needing a "Skip Animation" input.
  - Quest Board:
    - Automatically accelerates the camera zoom effect without needing a "Skip Animation" input.
    - Quest list loading delay removed.
  - Menu Lists (Item Box, NPC options, etc):
    - Removed delay between each option fading in.
  - Other UIs:
    - Intro and outro animations sped up.
- Item Loadout and Equipment Loadout maximum name length increased to 20 (up from 16).

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
  - Whetfish Fin and Whetfish Fin+ can be melded. The plus variant is unlocked in MR.
  - High Rank augment materials:
    - Any of the 7 types of Warrior's Streamstones can be melded from 2 Warrior's Streamstones of any other type.
    - Any of the 7 types of Hero's Streamstones can be melded from 2 Hero's Streamstones of any other type.
    - 2 Warrior's Streamstones can be melded from a single Hero's Streamstone of the same type.
    - Hero's Streamstones can be melded from 4 Warrior's Streamstones of the same type.
  - Guiding Lands materials:
    - Elder Dragonvein Bone can be melded from Elder Spiritvein Bone.
    - Dragonvein Solid Bone can be melded from Spiritvein Solidbone.
    - Heavy Dragonvein Bone can be melded from Spiritvein Slogbone.
    - > These options were added to allow hunters to directly downgrade tempered bones into non-tempered variants, similar to other Guiding Lands materials.
- Steamworks:
  - The time required to complete each three-button round has been drastically reduced.
- Kulve Taroth and the Safi'jiva Siege are no longer on rotation and are now permanently active.

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
Details for Monster Hitzone changes and Clutch Claw Softening are found near the top of [General Changes](#general-changes).

#### ──────────【 Alatreon 】────────── ####
Due to element damage output increasing significantly on many weapon types, Alatreon's weapon-specific element topple multipliers have been adjusted. A lower multiplier means a weapon's element damage will count for less and the hunter will need to deal more total element damage to reach each topple.
- Great Sword modifier decreased to 0.8x (down from 1.1x).
- Hunting Horn modifier decreased to 0.8x (down from 1.0x).

## Experimental General Changes ##

### Hunter Attack Turning ###
The following changes were made to increase the responsiveness of turning controls during combos. These changes only affect attacks that already support turning between attacks within a combo.
- Directional input angle deadzone reduced.
- Minimum turning angle removed.

## Experimental Weapon Changes ##
The changes below are in addition to (or overwrite) changes from Stable. See Stable's change log for full weapon details.

### ──────────【 Hammer 】────────── ###

#### 【 New Move: Power Charge Dash 】 ####
Power Charge Dash:
- While Power Charge state is active, using Power Charge again will perform a Power Charge Dash.
- Removes Power Charge state, but immediately upgrades current charge level to 3.
- After a 0.166s delay from starting the Dash, grants Hyper Armor for 2s.
- Can be comboed into Charge, or into any Charge follow-up moves.
- Combo options:
  - Big Bang IV can be performed after a Spinning Strong Upswing.
  - A half-variant of Brutal Big Bang can be performed by releasing the Charge input without a directional input.
  - Spinning Bludgeon can be performed by releasing the Charge input with a directional input.
  - Charge can be performed by holding the Charge input.

### ──────────【 Bow 】────────── ###

#### 【 Dragon Piercer 】 ####

Dragon Piercer has received a minor rework in an effort to increase its effectiveness across all matchups. It will be easier and safer to use throughout a hunt due to having a shorter animation, while providing damage on a wider range of Monsters that is comparable to other Bow attacks.

- Dragon Piercer:
  - Start up time reduced by approximately 33%.
  - Recovery animation for all levels changed to use the significantly shorter Level 1 version.
  - Delay between ticks decreased to 0.033s at all levels (down from 0.067s/0.067s/0.050s/0.050s).
  - MV decreased to 11/14/17/20 (down from 19/20/23/24).
  - Element Modifier increased to 0.3x/0.45x/0.6x/0.7x (up from 0.15x/0.2x/0.3x/0.3x).
  - Status Modifier increased to 0.4x/0.5x/0.6x/0.7x (up from 0.2x/0.25x/0.3x/0.3x).
  - Fixed Damage removed (was 1/1/2/2).
  - Damage and Buildup decreased to 4% after 18th hit (was 20%).


