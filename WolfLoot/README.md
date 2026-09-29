# WolfLoot

**Mod version:** 1.0.1  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

Version **1.0.1**. Tamed wolves collect nearby ground item drops into the nearest loaded chest marked by a sign whose first line is `wolf loot`. Wolves must be within the configured pickup radius of a drop and chest search radius of a marked chest. The mod transfers existing items; it does not generate loot.

## Install and configure

Install BepInEx for Valheim, copy `WolfLoot.dll` into `BepInEx/plugins`, and restart. For multiplayer, the default server-authoritative mode requires the DLL on the host or dedicated server.

BepInEx creates `BepInEx/config/com.JNP.wolfloot.cfg` after launch:

| Section | Key | Default | Purpose |
| --- | --- | --- | --- |
| General | `Enabled` | `true` | Enable collection. |
| General | `WolfNameContains` | `Wolf` | Creature object-name filter. |
| General | `ChestSignText` | `wolf loot` | First line of sign beside destination chest. |
| Loot | `PickupRadius` | `6` | Drop scan distance from each wolf, in meters. |
| Loot | `ChestSearchRadius` | `50` | Destination chest search distance, in meters. |
| Performance | `TickInterval` | `1` | Seconds between manager ticks. |
| Performance | `WolvesPerTick` | `10` | Maximum wolves scanned per tick. |
| Performance | `ChestCacheRefreshInterval` | `15` | Seconds between chest cache refreshes. |
| Performance | `MaxDropsPerWolf` | `5` | Maximum drops moved per wolf per scan. |
| Multiplayer | `ServerAuthoritative` | `true` | Let only the host/server transfer drops. |
| Debug | `DebugLogging` | `false` | Log transfer and cache details. |
