# BetterLandscaping

**Mod version:** 1.2.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

Adds **Square Level**, **Square Smooth**, **Circle Level**, **Circle Smooth**, and **Remove Tree** to the vanilla hoe menu.

## Use

1. Equip the hoe and open its build menu.
2. Select a square or circle shape, then **Level** for a flat center or **Smooth** for a softer transition at the edge.
3. Aim at the ground. The outline shows the complete area that can change.
4. Hold **Ctrl** and scroll to resize the brush. The default width matches the installed game's Level Ground tool (6 m in the tested Valheim build). Squares can be 2 to 16 m wide; circles can be 4 to 16 m wide, in 2 m steps.
5. Click to level toward the ground height under your character.

The square stays aligned with the terrain grid. Circles follow the grid, so their edges are approximate. All four tools paint dirt like the vanilla Level Ground tool. The preview is green when the target is within normal terrain limits and orange if some ground cannot reach that height. The tool costs no stone; normal hoe stamina and durability costs still apply.

The brush only edits terrain vertices whose visible triangles fit inside its outline. This reserves an edge band where changed and untouched terrain meet. Smooth modes blend inside the outline; Level modes aim for a flat center.

## Remove Tree

Select **Remove Tree** in the hoe menu, aim at a standing tree, fallen log, or stump, and click. The small green ring marks the object under the crosshair. An orange ring means a ward blocks removal. Each click removes one object and creates no wood, seeds, logs, or stump. Existing logs and stumps are separate objects and each needs its own click.

Removal uses normal hoe stamina and durability, costs no resources, and respects ward access. Objects marked effectively indestructible by the game are excluded. The mod deletes the selected network object directly so multiplayer peers see the same result; every player and the dedicated server should use the same mod version.

## Install

Install BepInEx for Valheim, then copy only `BetterLandscaping.dll` into `Valheim/BepInEx/plugins`. Install the same DLL on every client and the dedicated server. The mod uses BepInEx and Harmony.

There are no user-configurable settings or config file for this mod. Brush size is adjusted in game with Ctrl + mouse wheel.
