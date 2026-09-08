# CastleMiner Z — Player Skins

A client-side cosmetic skin mod for **CastleMiner Z 1.9.9.8** that expands the stock SWAT uniform into a large locally rendered appearance catalog while preserving the original player model, tactical gear, animations, and gameplay behavior.

> **Unofficial community project:** Player Skins is independently created and published by AnlionGamer. It is not an official CastleMiner Z release and is not affiliated with, sponsored by, approved by, or endorsed by the game's developers or publisher.

**Publisher:** AnlionGamer  
**Current release:** v1.4.1  
**Mod ID:** `cmz.player-skin-randomizer`

## Features

- **140 appearances:** 17 solid colors and 123 named camouflage appearances.
- Separate **My Skins** and **Other Players Skins** settings pages.
- Recolors garment cloth while excluding tactical gear from recoloring.
- Uses bounded source shading so folds and fabric detail remain visible instead of inheriting the stock navy brightness.
- Uses a geometry-derived garment mask covering the intended uniform UV islands, including collar, trouser hems, and sleeve cuffs.
- Populates mipmaps at every supported texture tier for better near/far texture filtering.
- Includes Manager previews for all 140 appearances, rendered from the actual CMZ player geometry and compiled mod texture output.
- Preserves all 140 stable skin IDs so existing v1.4.x selections remain valid.
- Cosmetic rendering remains local to the modded client; other players do not need Player Skins or CMZ Mod Manager.

## Appearance Catalog

v1.4.1 contains:

- **17 solid colors**
- **123 camouflage appearances** spanning U.S., Chinese, Taiwanese, Brazilian, Czech, Danish, Finnish, French, German, Greek, Hungarian, Italian, Japanese, Dutch, Norwegian, Polish, Romanian, Russian, South Korean, Spanish, Swedish, Turkish, Ukrainian, and other named pattern families represented in the catalog.

The camouflage artwork is an original procedural interpretation of the named patterns. It is not presented as an exact textile-print reproduction or a certification of every historical or specialist issue variant.

## Requirements

- CastleMiner Z **1.9.9.8** (Steam)
- CMZ Mod Manager **1.2.0 or newer**
- CMZ Mod Framework/API **1.0.0 or newer**
- Windows / x86 game process

## Installation

1. Download `CMZ_Player_Skins_v1.4.1.cmzmod` from the GitHub Releases page.
2. Install the `.cmzmod` through CMZ Mod Manager.
3. Enable **Player Skins** in the active profile.
4. Configure **My Skins** and **Other Players Skins** if desired.
5. Launch CastleMiner Z through the Mod Manager.

Installing v1.4.1 updates the existing Player Skins mod identity rather than creating a second mod.

## Settings

### My Skins

- **Nothing checked:** Random from the full appearance catalog.
- **One checked:** Always use that appearance for the local player.
- **Multiple checked:** Randomly choose only from the checked appearances for each new match/session.

### Other Players Skins

These choices affect only how remote players appear **on your screen**.

- **Nothing checked:** Random from the full appearance catalog.
- **One checked:** Show other players with that selected appearance locally.
- **Multiple checked:** Assign remote players only from the selected pool.

For restricted remote pools, available choices are exhausted before reuse.

Older `appearanceMode` / `selectedSkins` preferences remain a compatibility fallback when the newer `mySkins` setting is absent.

## v1.4.1 Visual Corrections

- Palette-driven cloth shading replaces the old stock-navy brightness dependency.
- White and snow oversuits stay white instead of becoming gray or navy-biased.
- U.S. and Dutch Three-Color Desert patterns use three base colors.
- UCP uses three base colors.
- OCP and OEF-CP / MultiCam use seven color roles with blended background fields and smaller body patches.
- Flecktarn distribution and sand-dominant Tropentarn were revised.
- French BME transitions and pale branch forms were revised.
- Norway First Entry earth colors were revised.
- Flora now uses horizontal forms; VSR-93 remains vertical. Both use three base colors.
- Garment coverage was corrected around dark shirt areas, collar, trouser hems, and sleeve cuffs while keeping gear excluded.
- Generated textures now include populated mip chains through 1x1.

## Multiplayer

Player Skins is designed as a **client-side cosmetic mod**.

The mod does not add custom multiplayer messages, modify CastleMiner Z's network protocol, or require other players to install Player Skins, CMZ Mod Manager, or the CMZ Mod Framework.

The skins seen on remote players are generated and displayed by the modded client's game. Cosmetic assignments are not transmitted to vanilla clients.

The earlier v1.3.3 release was runtime-tested in multiplayer for approximately 33 minutes with one local player and two remote players receiving distinct locally rendered skins and a normal session shutdown. That historical test does **not** substitute for live-game validation of the expanded v1.4.1 visual catalog.

## v1.4.1 Validation Status

The v1.4.1 payload passed compiled offline checks covering:

- 140 unique catalog IDs,
- stable-ID parsing and deduplication,
- current settings and legacy fallback behavior,
- fixed local single-choice behavior,
- restricted and unrestricted remote skin-pool behavior,
- RGBA upload behavior,
- full mip upload through reflective API-shaped test doubles,
- and texture disposal after failed partial upload.

The package privacy guard passed. The final release archive's declared payload SHA-256 hashes were reverified after the license correction, and the `.cmzmod` now carries the full `LICENSE.txt` and `NOTICE.md` as declared, hashed payload files.

**Not yet claimed for v1.4.1:** live CastleMiner Z / XNA graphics-device appearance testing, joining behavior, or Windows frame-rate measurement.

## Privacy

- No telemetry or analytics.
- No web requests or data uploads.
- No custom multiplayer traffic.
- No local user-profile or PDB/debug paths in the release DLL.
- Player identity information used for session-local appearance bookkeeping is not intended to be logged, persisted, or transmitted by the mod.

## Save / Removal Safety

Player Skins does not intentionally modify world data, player progression, inventories, or save formats. Disable or remove it through CMZ Mod Manager. Existing saves are not expected to require conversion.

## Repository Policy

This repository is for **public releases and finished public-facing states only**. Development builders, intermediate test builds, dependencies, diagnostics, and private build artifacts are intentionally excluded.

The reference manifest for each public release is kept under `Release/`. Installable `.cmzmod` packages belong on the GitHub **Releases** page rather than in the repository tree. Current release packages carry their applicable license and project notice inside the `.cmzmod` so those terms remain attached when the package is shared separately from GitHub.

## License and Attribution

Player Skins **v1.4.1 and the current repository state** are governed by the **AnlionGamer Community Distribution Terms v1.0**. See [`LICENSE`](LICENSE).

The terms allow normal use, source inspection where source is published, and private modification. Public redistribution of the original project, packaged mod, forks, or modified builds requires **prior permission from AnlionGamer** and must remain **non-commercial**. Sale and paid access are prohibited without separate permission.

**Historical license:** Player Skins v1.3.3 and earlier copies already published under the MIT License retain the MIT permissions that accompanied those copies. See [`LICENSE_HISTORY.md`](LICENSE_HISTORY.md).

The original Player Skins mod concept, design direction, and release are credited to **AnlionGamer**. Additional project attribution and the CastleMiner Z rights notice are documented in [`NOTICE.md`](NOTICE.md).

CastleMiner Z and its original game assets remain the property of their respective rights holders. This is an independent, unofficial fan-made mod project and is not affiliated with or endorsed by the game's rights holders.

## Release Integrity

Current v1.4.1 package:

`CMZ_Player_Skins_v1.4.1.cmzmod`

SHA-256:

`60529bb4d539f3946ca368b9c760c4b0f4eab1597eef09a839a24f7f28a3c269`

A matching `SHA256SUMS.txt` is provided for release verification.
