# Castle Miner Z — Player Skins

A client-side cosmetic skin mod for **Castle Miner Z 1.9.9.8** that recolors the stock SWAT uniform while preserving the original player model, texture detail, tactical gear, animations, and gameplay.

> **Unofficial community project:** Player Skins is independently created and published by AnlionGamer. It is not an official Castle Miner Z release and is not affiliated with, sponsored by, approved by, or endorsed by the game's developers or publisher.

**Publisher:** AnlionGamer  
**Current release:** v1.3.3  
**Mod ID:** `cmz.player-skin-randomizer`

## Features

- 17 solid-color player appearances generated from Castle Miner Z's stock SWAT diffuse texture.
- Recolors the uniform cloth only; tactical gear, boots, vest, straps, pads, gloves, helmet, and other non-uniform details remain vanilla-colored.
- Preserves the original Castle Miner Z player model, geometry, UV mapping, normal/specular behavior, animations, and gameplay behavior.
- Assigns players distinct locally rendered skins from a shuffled pool while unused skins remain available.
- Lets the local player use the normal random assignment or select one or more preferred skins.
- Cosmetic rendering is local to the modded client and does not require other players to install the mod or CMZ Mod Manager.

## Available Skins

- White
- Coral Red
- Copper Orange
- Mustard Gold
- Forest Green
- Steel Blue
- Periwinkle
- Orchid
- Gray
- Crimson Red
- Burnt Orange
- Olive
- Dark Green
- Navy Blue
- Indigo
- Purple
- Charcoal Black

## Requirements

- Castle Miner Z **1.9.9.8** (Steam)
- CMZ Mod Manager **1.1.1 or newer**
- CMZ Mod Framework/API **1.0.0 or newer**
- Windows / x86 game process

## Installation

1. Download `CMZ_Player_Skins_v1.3.3.cmzmod` from the GitHub Releases page.
2. Install the `.cmzmod` through CMZ Mod Manager.
3. Enable **Player Skins** in the active profile.
4. Configure **My Skin** if desired.
5. Launch Castle Miner Z through the Mod Manager.

## Settings

### My Skin

- **Random** — uses the normal shuffled skin pool.
- **Select Skin(s)** — uses only the local player's selected personal skins.

### Selected Skin(s)

When **My Skin** is set to **Select Skin(s)**:

- Selecting one skin keeps that skin for the local player.
- Selecting multiple skins randomly chooses among those selected skins for each new local match/session.

## Multiplayer

Player Skins is designed as a **client-side cosmetic mod**.

The mod does not add custom multiplayer messages, modify Castle Miner Z's network protocol, or require other players to install Player Skins, CMZ Mod Manager, or the CMZ Mod Framework.

Real multiplayer testing of v1.3.3 was successful. In a normal multiplayer session:

- the local player received a personal skin,
- two remote players received different locally rendered skins,
- no skin was duplicated among the three observed players,
- normal gameplay continued without visible disruption to the other players,
- a departing player's local cosmetic assignment was cleaned up,
- and the approximately 33-minute test session shut down normally.

The skins seen on remote players are generated and displayed by the modded client's game. The mod does not transmit those cosmetic assignments to vanilla clients.

## Privacy

The v1.3.3 release package was checked before publication for accidental private build information and unnecessary data handling.

- No telemetry or analytics.
- No web requests or data uploads.
- No custom network traffic.
- No local user-profile or PDB/debug paths in the release DLL.
- Player identity information used for session-local assignment bookkeeping is not logged, persisted, or transmitted by the mod.

## Save / Removal Safety

Player Skins does not intentionally modify world data, player progression, inventories, or save formats. Disable or remove it through CMZ Mod Manager. Existing saves are not expected to require conversion.

## Repository Policy

This repository is for **public releases and finished states only**. Development builders, intermediate test builds, dependencies, diagnostics, and private build artifacts are intentionally excluded.

The reference manifest for the current public release is included under `Release/`. Installable `.cmzmod` packages belong on the GitHub **Releases** page rather than in the repository tree.

Future Player Skins release packages should carry their applicable license and project notice inside the `.cmzmod` package so the terms remain attached when the package is shared separately from GitHub.

## License and Attribution

The current repository `main` branch and future Player Skins work are governed by the **AnlionGamer Community Distribution Terms v1.0**. See [`LICENSE`](LICENSE).

The terms allow normal use, source inspection, and private modification. Public redistribution of the original project, source, packaged mod, forks, or modified builds requires **prior permission from AnlionGamer** and must remain **non-commercial**. Sale and paid access are prohibited without separate permission.

**Historical license:** Player Skins v1.3.3 and earlier copies already published under the MIT License retain the MIT permissions that accompanied those releases. Relicensing the repository going forward does not revoke those historical permissions. See [`LICENSE_HISTORY.md`](LICENSE_HISTORY.md).

The original Player Skins mod concept, design direction, and release are credited to **AnlionGamer**. Additional project attribution and the Castle Miner Z rights notice are documented in [`NOTICE.md`](NOTICE.md).

Castle Miner Z and its original game assets remain the property of their respective rights holders. This is an independent, unofficial fan-made mod project and is not affiliated with or endorsed by the game's rights holders.

## Release Integrity

Current v1.3.3 package:

`CMZ_Player_Skins_v1.3.3.cmzmod`

SHA-256:

`46061b42017ca79da796c234e428394e9f13fa8288fa7582d7476266a17da484`

Release downloads should include `SHA256SUMS.txt` so the package can be verified after download.
