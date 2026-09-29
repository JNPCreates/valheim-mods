# Portal Directory

**Mod version:** 1.0.1  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

Version **1.0.1**. Turn a normal sign into a portal directory by making its first line `portal directory`, then interact with it. The window lists portal names, counts, and whether each name appears matched. The count is a simple name count, not a check that a portal pair can be used.

## Install and configure

Install BepInEx for Valheim, copy `PortalDirectory.dll` into `BepInEx/plugins`, and restart. For the server-wide portal list in multiplayer, install the same DLL on the server and on players who will open the directory. Otherwise a client may see only locally known portals.

BepInEx creates `BepInEx/config/com.JNP.portaldirectory.cfg` after launch:

| Key in `[General]` | Default | Purpose |
| --- | --- | --- |
| `DirectorySignText` | `portal directory` | Text on the first line of a directory sign; matching ignores case. |
| `CacheSeconds` | `120` | How long to keep a scanned portal list before rescanning. |
