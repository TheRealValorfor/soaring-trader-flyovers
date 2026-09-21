# Soaring Trader Flyovers

**CurseForge:** [soaring-trader-flyovers](https://www.curseforge.com/minecraft/data-packs/soaring-trader-flyovers)

A datapack for **Create Aeronautics: Discovery** on Minecraft 1.21.1. Soaring Traders spawn higher, fly with terrain and obstacle avoidance, and skip the worst mountain biomes so biplanes spend less time in your base.

The CurseForge file listing was not public yet when this README was last synced from the live API.

## Requires

- Minecraft 1.21.1
- [Create Aeronautics: Discovery](https://www.curseforge.com/minecraft/mc-mods/create-aeronautics-discovery) (`1580189`)

**Optional:** [Moonlight Lib](https://www.curseforge.com/minecraft/mc-mods/selene) (`499980`) — only if you want instance-root `datapacks/` applied to every world. Vanilla install is a world’s `datapacks` folder and does not need Moonlight.

## What it changes

- Trader and pillager flyovers spawn at Y 280–310
- Cruise altitude 250–305 with straight, altitude, terrain (24-block clearance), and avoid goals
- Woodland mansion and pillager outpost patrols spawn at Y 240–250 with the same avoid behaviour
- Skips jagged, frozen, and stony peaks, windswept savanna, and `*:*mountain*` biomes

This datapack does **not** change flyover lifetime. That is still `aeronauticsdiscovery-common.toml` (`maxLifetimeTicks`).

## Install

CurseForge app: **Add More Content → Data Packs**. That drops the zip into the instance `datapacks/` folder.

Manual: copy `SoaringTraderFlyovers-1.0.0.zip` into the instance `datapacks/` folder (not `saves/<world>/datapacks` unless you are not using Moonlight). Then restart.

To rebuild the zip from this repo:

```bash
zip -r SoaringTraderFlyovers-1.0.0.zip pack.mcmeta data
```

## Limits

Planes can still hit a tall build. If a player gets within one block of a flyover, Discovery hands the wreck to Sable and that vehicle no longer uses the flyover despawn timer.

## Changelog 1.0.0

- Flyover spawn Y 280–310; cruise altitude 250–305
- Autopilot: straight + altitude + terrain (24-block clearance) + avoid
- Pillager mansion/outpost patrols raised to Y 240–250 with the same avoid goals
- Exclude jagged/frozen/stony peaks, windswept savanna, and `*:*mountain*` biomes
