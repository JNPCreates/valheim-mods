# Storage Directory

**Mod version:** 1.0.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

Version **1.0.0**. Turn a normal sign into a searchable storage list by making its first line `storage directory`, then interact with it. The list totals items in **loaded** nearby containers; distant or unloaded chests are not included. It displays counts and does not move items.

## Install and configure

Install BepInEx for Valheim, copy `StorageDirectory.dll` into `BepInEx/plugins`, and restart the game. Install it on each player who will use the directory. BepInEx creates `BepInEx/config/com.JNP.storagedirectory.cfg` after launch:

| Key in `[General]` | Default | Purpose |
| --- | --- | --- |
| `DirectorySignText` | `storage directory` | Text on the first line of a directory sign; matching ignores case. |
| `ScanRadius` | `50` | Meters around the sign to scan loaded containers. |
| `GroupByQuality` | `true` | List different quality levels separately. |
| `SortMode` | `Name` | Sort by `Name` or `Count`. |
