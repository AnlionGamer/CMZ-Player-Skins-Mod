# Changelog

## v1.4.1 — Expanded Catalog and Visual Corrections

- Expanded Player Skins from 17 solid appearances to **140 total appearances**: 17 solid colors and 123 camouflage appearances.
- Added separate **My Skins** and **Other Players Skins** settings pages.
- Preserved all 140 stable skin IDs and compatibility fallback for older `appearanceMode` / `selectedSkins` settings.
- Reworked cloth recoloring so named RGB palettes control the fabric color while bounded source shading preserves folds and texture detail.
- Corrected white and snow oversuits so they remain white rather than inheriting the stock navy brightness.
- Corrected U.S. and Dutch Three-Color Desert patterns to use three base colors.
- Corrected UCP to use three base colors.
- Reworked OCP and OEF-CP / MultiCam to use seven color roles with blended background fields and smaller body patches.
- Revised Flecktarn distribution and sand-dominant Tropentarn.
- Revised French BME transitions and pale branch forms.
- Revised Norway First Entry earth colors.
- Changed Flora to horizontal forms while keeping VSR-93 vertical; both use three base colors.
- Added a geometry-derived garment mask covering eight intended uniform UV islands, including dark shirt areas, trouser hems, and sleeve cuffs while excluding tactical gear.
- Added populated mip chains through 1x1 at every supported texture tier.
- Rebuilt all 140 Manager previews using the actual CMZ player geometry and texture bytes emitted by the compiled mod.
- Preserved square pattern swatches in preview presentation.
- Compiled offline tests passed for catalog identity, settings migration, local selection behavior, remote pool behavior, RGBA upload, mip upload, and failed-upload disposal.
- Package privacy guard passed and declared payload hashes were reverified for the final release archive.
- Live CastleMiner Z / XNA graphics-device validation and Windows performance measurement are not claimed for v1.4.1.
- v1.4.1 is distributed under the **AnlionGamer Community Distribution Terms v1.0**. Historical v1.3.3 and earlier MIT-distributed copies retain their original MIT permissions.

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
