# CraftingFromStorage

**Mod version:** 1.0.2  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

**Mod version:** 1.0.2

Lets crafting and upgrading use materials in nearby, accessible containers. It checks your inventory first, then searches containers within 10 meters by default. Hammer building is disabled by default.

## Install

Install BepInEx for Valheim, then place `CraftingFromStorage.dll` in `BepInEx/plugins` and start the game.

## Configure

BepInEx creates `BepInEx/config/com.JNP.craftingfromstorage.cfg` after the first launch.

| Section | Setting | Default | Purpose |
| --- | --- | --- | --- |
| General | `Enabled` | `true` | Turn the mod on or off. |
| General | `PullRadius` | `10` | Container search radius in meters. |
| General | `IncludeCrafting` | `true` | Use storage for crafting and upgrading. |
| General | `IncludeBuilding` | `false` | Use storage for hammer building. |
| General | `PullClosestFirst` | `true` | Search closest containers first. |
| General | `LeaveOneInStorage` | `false` | Keep one item of each pulled type in a container when possible. |
| Containers | `RequirePlayerBuiltContainers` | `true` | Ignore containers without a player-built piece. |
| Containers | `IgnoreCarts` | `true` | Ignore cart containers. |
| Containers | `IgnoreShips` | `true` | Ignore ship containers. |
| Debug | `DebugLogging` | `false` | Add pull and count messages to the BepInEx log. |

The mod skips containers that are in use or inaccessible to the player.
