# CameraTweaks

**Mod version:** 1.0.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

**Mod version:** 1.0.0

Extends the camera zoom distance and lets you enter a close first-person view by scrolling inward past the normal minimum. Scroll outward to return to third person. Extended zoom defaults to 12 units on foot and 18 while controlling a ship.

## Install

Install BepInEx for Valheim, then place `CameraTweaks.dll` in `BepInEx/plugins` and start the game.

## Configure

BepInEx creates `BepInEx/config/com.JNP.CameraTweaks.cfg` after the first launch. In `[Extended Zoom]`, use `Enabled`, `MaxDistance`, and `MaxBoatDistance`. In `[First Person]`, use `Enabled`, `ScrollsPastMinToEnterFirstPerson`, `FirstPersonDistance`, `FirstPersonOffsetX/Y/Z`, `FirstPersonNearClipPlane`, and `ExitFirstPersonDistance`. In `[Fake First Person]`, `OverrideThirdPersonOffsets` and the `ThirdPersonOffsetX/Y/Z` and `ThirdPersonCombatOffsetX/Y/Z` settings adjust the close camera when `FirstPersonDistance` is above zero. Defaults enable both zoom and first person; first person starts after one extra inward scroll.
