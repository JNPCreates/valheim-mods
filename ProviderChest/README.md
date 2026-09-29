# Provider Chest

**Mod version:** 1.0.1  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

Version **1.0.1**. A player-built chest with a nearby sign reading exactly `provider` becomes a supply chest. After a player successfully places a building piece, the chest tries to refill item types the player already carries, up to one maximum stack per type. It takes those items from the chest; it does not create them.

## Install and configure

Install BepInEx for Valheim, copy `ProviderChest.dll` into `BepInEx/plugins`, and restart. BepInEx creates `BepInEx/config/com.yourname.providerchest.cfg` after launch. The plugin ID contains `yourname` in this version.

| Key in `[General]` | Default | Purpose |
| --- | --- | --- |
| `PlayerRange` | `10` | Maximum distance from player to provider chest at placement. |
| `SignRadius` | `2` | Maximum distance from chest to its `provider` sign. |
