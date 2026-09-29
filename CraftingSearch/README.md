# CraftingSearch

**Mod version:** 1.0.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

**Mod version:** 1.0.0

Adds a search box to the inventory crafting interface. Typing filters visible recipe rows by their displayed text. Matching recipes can be moved to the top of the list.

## Install

Install BepInEx for Valheim, then place `CraftingSearch.dll` in `BepInEx/plugins` and start the game.

## Configure

BepInEx creates `BepInEx/config/com.JNP.CraftingSearch.cfg` after the first launch. `[General] Enabled` controls the search box, `FocusOnOpen` focuses it when the interface opens, and `CompactResults` moves matches into the first visible slots. Defaults are `true`, `false`, and `true` respectively.

In `[Layout]`, `PlaceBesideUpgradeTab` places the box by the Craft/Upgrade tabs when available. `SearchBoxOffsetX2`, `SearchBoxOffsetY2`, `SearchBoxWidth2`, and `SearchBoxHeight2` adjust that placement. `FallbackSearchBoxX` and `FallbackSearchBoxY` set its position if the tab cannot be found.
