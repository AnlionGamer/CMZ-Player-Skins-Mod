# Changelog

## v1.3.3 — Initial Public Release

- Added 17 solid-color player skins generated from Castle Miner Z's official SWAT diffuse texture.
- Recolors only identified uniform cloth while preserving tactical gear and other non-uniform details.
- Preserves the official player model, geometry, UV mapping, normal/specular behavior, animations, and gameplay behavior.
- Added **Random** and **Select Skin(s)** local-player appearance modes.
- Supports selecting one fixed personal skin or a pool of preferred skins for new sessions.
- Uses a shuffled local skin pool so active players receive distinct appearances while unused skins remain available.
- Corrected the persistent dark crotch/inner-thigh recolor artifact before public release while preserving the vanilla uniform's shading and texture detail.
- Runtime-tested in multiplayer with one local player and two remote players receiving distinct locally rendered skins.
- Multiplayer test continued for approximately 33 minutes and shut down normally.
- Does not add custom multiplayer messages or modify Castle Miner Z's multiplayer traffic or protocol.
- Other players do not need Player Skins, CMZ Mod Manager, or the CMZ Mod Framework for the modded client to display local cosmetic assignments.
- Release package privacy-checked for accidental user-profile paths, PDB/debug paths, telemetry, web/data-upload behavior, and unnecessary persistence of player identity information.
- Public release targets Castle Miner Z **1.9.9.8** and requires CMZ Mod Manager **1.1.1+**.
