# AutoCloseDoors

**Mod version:** 1.0.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

BepInEx/Harmony mod that closes existing Valheim doors and gates after **120 seconds**. No new building piece or recipe is required. Doors that require keys or are marked by the game as unable to close are excluded.

## Configuration

After the first launch with the mod installed, edit `BepInEx/config/com.JNP.AutoCloseDoors.cfg` with the game closed:

```ini
[General]
Enabled = true
CloseDelaySeconds = 120
```

The delay accepts 1–3600 seconds. Closing and reopening a door starts a fresh timer. Already open doors start their timer when they load. Timers run during active gameplay, pause with the game, and restart when a door unloads or the world reloads. Sleeping does not skip the countdown. An opening animation must finish before the mod can close the door.

In multiplayer, only the peer that owns the door changes its state. Install on every player's game and on a dedicated server, if used, with matching configuration; configuration is local and is not automatically synchronized. Timers are tracked on each peer while the door is loaded, so a newly arriving peer can have a later countdown. Normal game networking distributes the closed state and the normal door code plays its animation and effects.

## Install

Install BepInEx for Valheim. With the game closed, copy `AutoCloseDoors.dll` into `Valheim/BepInEx/plugins`, then start the game. BepInEx creates the config file on first launch. Do not copy game or Unity DLLs from a build directory.

Remove `AutoCloseDoors.dll` to uninstall. This mod adds no custom pieces or persistent world data.
