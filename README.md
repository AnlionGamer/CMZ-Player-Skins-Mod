# Castle Miner Z — Player Skins

A client-side cosmetic skin mod for **Castle Miner Z 1.9.9.8** that recolors the official SWAT uniform while preserving the original player model, texture detail, tactical gear, animations, and gameplay.

**Publisher:** AnlionGamer  
**Current release:** v1.3.3  
**Mod ID:** `cmz.player-skin-randomizer`

## Features

- 17 solid-color player appearances generated from Castle Miner Z's official SWAT diffuse texture.
- Recolors the uniform cloth only; tactical gear, boots, vest, straps, pads, gloves, helmet, and other non-uniform details remain vanilla-colored.
- Preserves the official player model, geometry, UV mapping, normal/specular behavior, animations, and gameplay behavior.
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

## License and Attribution

Player Skins is released under the **MIT License**. See [`LICENSE`](LICENSE) for the complete license text.

The original Player Skins mod concept, design direction, and release are credited to **AnlionGamer**. The MIT License requires its copyright and permission notice to remain with copies or substantial portions of the software. Additional project attribution and the Castle Miner Z rights notice are documented in [`NOTICE.md`](NOTICE.md).

Castle Miner Z and its original game assets remain the property of their respective rights holders. This is an independent, unofficial fan-made mod project and is not affiliated with or endorsed by the game's rights holders.

## Release Integrity

Current v1.3.3 package:

`CMZ_Player_Skins_v1.3.3.cmzmod`

SHA-256:

`46061b42017ca79da796c234e428394e9f13fa8288fa7582d7476266a17da484`

Release downloads should include `SHA256SUMS.txt` so the package can be verified after download.
