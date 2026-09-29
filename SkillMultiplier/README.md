# SkillMultiplier

**Mod version:** 1.0.0  
**Built for:** Valheim 1.0.16 with BepInExPack 5.4.2350. Gameplay and multiplayer features need further testing.

Version **1.0.0**. Multiplies the amount passed to Valheim's skill gain method for every skill. The default is double gain; `1` restores vanilla gain and negative settings are treated as zero.

## Install and configure

Install BepInEx for Valheim, copy `SkillMultiplier.dll` into `BepInEx/plugins`, and restart the game. BepInEx creates `BepInEx/config/com.JNP.SkillMultiplier.cfg` after launch. Set `[General] SkillGainMultiplier` to the desired multiplier (default `2.0`). Each player's game needs the DLL for that player's skill gains.
