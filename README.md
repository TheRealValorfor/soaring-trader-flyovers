# Soaring Trader Flyovers

CurseForge **datapack** export. Requires **Create Aeronautics: Discovery** (NeoForge 1.21.1).

Raises Soaring Trader (and pillager) flyovers, adds terrain/avoid autopilot, and skips some mountain biomes so planes crash less. Does **not** change Discovery’s 4-minute lifetime — that lives in `aeronauticsdiscovery-common.toml`.

## Upload

File: **`SoaringTraderFlyovers-1.0.0.zip`**

- Project type: **Customization → Data Packs**
- Game versions: **1.21.1**
- Mod loaders: leave empty or mark as datapack (not a NeoForge mod)
- Relation: required **Create Aeronautics: Discovery**

Do **not** tick this folder in a Worlds Further **modpack** export. The pack installs the same zip at instance `datapacks/` (CurseForge Data Packs path). Moonlight’s `global_datapacks_folder` is `datapacks`.

## Install (standalone)

CurseForge app: **Add More Content → Data Packs**. That drops the zip into the instance `datapacks/` folder.

Manual: copy `SoaringTraderFlyovers-1.0.0.zip` into the instance `datapacks/` folder (not `saves/<world>/datapacks` unless you are not using Moonlight). Then restart.

## Summary (paste)

Soaring Trader biplanes spawn higher (Y 280–310), cruise with terrain and obstacle avoidance, and skip jagged/frozen/stony peaks. For Create Aeronautics: Discovery on Minecraft 1.21.1.

## Changelog 1.0.0 (paste)

- Flyover spawn Y 280–310; cruise altitude 250–305
- Autopilot: straight + altitude + terrain (24-block clearance) + avoid
- Pillager mansion/outpost patrols raised to Y 240–250 with the same avoid goals
- Exclude jagged/frozen/stony peaks, windswept savanna, and `*:*mountain*` biomes
