# Hopper Chest

**Mod version:** 1.0.1  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

**Mod version:** 1.0.1

Turns a player-crafted chest into a sorting hopper when a nearby sign says exactly `hopper` (case insensitive). When you close the chest, it moves its items into nearby containers that already hold the same item type, checking the closest matching containers first. A background check also runs periodically.

## Install

Install BepInEx for Valheim, then place `HopperChest1stMod.dll` in `BepInEx/plugins` and start the game. The DLL name differs from the mod's display name.

Place a sign within 2 units of the hopper chest and set its text to `hopper`. Place destination containers within 8 units and stock each with at least one item of the type you want sorted there. Sorting runs when the hopper closes or at the background interval, provided the hopper has items.

## Configure

BepInEx creates `BepInEx/config/com.JNP.hopperchest.cfg` after the first launch. In `[General]`, `BackgroundTickInterval` defaults to 60 seconds, `SearchRadius` defaults to 8 units, and `SignRadius` defaults to 2 units.
