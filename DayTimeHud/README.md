# DayTimeHud

**Mod version:** 1.0.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

**Mod version:** 1.0.0

Displays the current Valheim day and elapsed time within that day in a small panel near the minimap. The time is based on Valheim's day cycle, not a real-world clock.

## Install

Install BepInEx for Valheim, then place `DayTimeHud.dll` in `BepInEx/plugins` and start the game.

## Configure

BepInEx creates `BepInEx/config/com.JNP.DayTimeHud.cfg` after the first launch.

| Section | Settings | Purpose |
| --- | --- | --- |
| Display | `ShowDay`, `ShowTime`, `ShowBackground`, `ReverseTextOrder` | Choose the text, background, and text order. |
| Position | `PlaceBelowMinimap` | Place the panel below the minimap instead of above it. |
| Style | `FontSize`, `FontName`, `FontColor`, `BackgroundColor`, `TextOutline`, `OutlineColor` | Change the panel text and colors. |
| Layout | `PanelWidth`, `PanelHeight`, `XOffset`, `YOffset`, `Padding` | Change panel size, position, and spacing. |
