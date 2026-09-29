# PlantGrid

**Mod version:** 1.0.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

Version **1.0.0**. Draws a terrain-following grid around the player to help align planting. The overlay starts hidden; press **Left Alt + G** to toggle it with the default shortcut.

## Install and configure

Install BepInEx for Valheim, copy `PlantGrid.dll` into `BepInEx/plugins`, and restart the game. BepInEx creates `BepInEx/config/com.JNP.PlantGrid.cfg` after the first launch. Edit these settings there:

| Section | Key | Default | Purpose |
| --- | --- | --- | --- |
| General | `ToggleShortcut` | Left Alt + G | Toggle the overlay. |
| General | `StartEnabled` | `false` | Show the overlay when a world loads. |
| Grid | `GridSpacing` | `1` | Meters between lines. |
| Grid | `GridRadius` | `12` | Cells drawn outward from the player. |
| Grid | `GroundOffset` | `0.04` | Lifts lines above the ground. |
| Grid | `GroundProbeHeight` | `80` | Height used to find ground below each point. |
| Visuals | `LineColor`, `AxisLineColor` | Green, yellow | Normal and center-line colors. |
| Visuals | `ShowAxisLines` | `true` | Highlight center lines. |
