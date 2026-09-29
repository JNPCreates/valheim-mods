# WolfPatrol

**Mod version:** 1.0.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

Version **1.0.0**. A tamed wolf commanded to stay will return toward its saved patrol point if it wanders too far. It pauses the return while the wolf follows a target or fights.

## Install and configure

Install BepInEx for Valheim, copy `WolfPatrol.dll` into `BepInEx/plugins`, and restart. For multiplayer, the default server-authoritative setting requires installation on the host or dedicated server.

BepInEx creates `BepInEx/config/com.JNP.WolfPatrol.cfg` after launch:

| Section | Key | Default | Purpose |
| --- | --- | --- | --- |
| General | `Enabled` | `true` | Enable return behavior. |
| General | `WolfNameContains` | `Wolf` | Creature object-name filter. |
| Patrol | `ReturnRadius` | `45` | Distance from patrol point that starts the return, in meters. |
| Patrol | `HomeArrivalDistance` | `8` | Distance at which the return ends, in meters. |
| Patrol | `RunHome` | `true` | Run toward the patrol point. |
| Multiplayer | `ServerAuthoritative` | `true` | Let only the host/server direct movement. |
