# BetterSmelting

**Mod version:** 1.0.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

One BepInEx/Harmony mod with separately configurable charcoal kiln output and smelting speed.

- Charcoal kilns produce **2 coal per wood** at their normal processing speed.
- Smelters and blast furnaces process ore at **2x speed**, with the same coal requirement per ingot.
- Existing and newly built stations are supported. Other production buildings are unaffected.

## Configuration

Close Valheim before editing `BepInEx/config/com.JNP.BetterSmelting.cfg`, then restart:

```ini
[General]
Enabled = true

[Kiln]
Enabled = true
CoalPerWood = 2

[Smelting]
Enabled = true
SpeedMultiplier = 2
```

`CoalPerWood` accepts integers from 1 to 10. `SpeedMultiplier` accepts values from 0.25 to 10. Set either to 1 to restore normal behavior for that feature, or disable its section. The General switch disables both features. Kiln output applies to its existing wood-to-coal recipes; this mod does not add recipes or accept new wood types.

The game processes these stations in one-second steps. Adjusted smelting time rounds up to a whole second so fractional settings do not waste additional fuel per ingot. For example, 30 seconds becomes 15 at 2x, or 8 at 4x. Fuel is consumed faster in real time because production is faster; its cost per ingot is unchanged. Smoke blockage and the game's normal processing and offline catch-up rules still apply.

## Install and remove

Install BepInEx for Valheim. With the game closed, copy `BetterSmelting.dll` to `Valheim/BepInEx/plugins`, then start the game. BepInEx creates the config with the defaults on first launch. Do not copy game or Unity reference DLLs from a build directory.

In multiplayer, install on every player's game and on the dedicated server, if used, with matching settings. Configuration is local and is not automatically synchronized. Only the station's network owner awards bonus coal. Every peer initializes the same smelting time so ownership changes preserve the configured rate.

Remove `BetterSmelting.dll` while the game is closed to uninstall. Normal processing returns on the next launch; coal already produced remains. The mod adds no custom items, building pieces or save fields. Avoid another mod changing these same production settings at the same time.
