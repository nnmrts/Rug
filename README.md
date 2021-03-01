# Rug Mod for Fabric

[![GitHub all releases](https://img.shields.io/github/downloads/RubixDev/fabric-rug/total)](https://github.com/RubixDev/fabric-rug/releases)
[![GitHub release (latest by date)](https://img.shields.io/github/downloads/RubixDev/fabric-rug/latest/total)](https://github.com/RubixDev/fabric-rug/releases/latest)
[![License](https://img.shields.io/github/license/RubixDev/fabric-rug)](https://github.com/RubixDev/fabric-rug/blob/main/LICENSE)
[![GitHub issues](https://img.shields.io/github/issues/RubixDev/fabric-rug)](https://github.com/RubixDev/fabric-rug/issues)
[![GitHub closed issues](https://img.shields.io/github/issues-closed/RubixDev/fabric-rug)](https://github.com/RubixDev/fabric-rug/issues?q=is%3Aissue+is%3Aclosed)
[![CurseForge All Versions](http://cf.way2muchnoise.eu/versions/For%20MC_449938_all.svg)](https://www.curseforge.com/minecraft/mc-mods/fabric-rug)
[![CurseForge Total Downloads](http://cf.way2muchnoise.eu/full_449938_downloads.svg)](https://www.curseforge.com/minecraft/mc-mods/fabric-rug)

Extension Mod for [gnembon's fabric-carpet](https://github.com/gnembon/fabric-carpet) with some more features

## Index
Count: 31
- [anvilledBlueIce](#anvilledblueice)
- [anvilledIce](#anvilledice)
- [anvilledPackedIce](#anvilledpackedice)
- [cactusFurnaceXP](#cactusfurnacexp)
- [concreteConvertOnCauldron](#concreteconvertoncauldron)
- [dragonDropsElytra](#dragondropselytra)
- [easyHarvesting](#easyharvesting)
- [easyHarvestingRequireHoe](#easyharvestingrequirehoe)
- [edibleGoldIngots](#ediblegoldingots)
- [edibleMagmaCream](#ediblemagmacream)
- [edibleNetheriteScraps](#ediblenetheritescraps)
- [edibleSlimeBalls](#edibleslimeballs)
- [enderPearlDamage](#enderpearldamage)
- [foodInstantHeal](#foodinstantheal)
- [lilyPadsOnCauldron](#lilypadsoncauldron)
- [newShulkerBehavior](#newshulkerbehavior)
- [noCreeperGriefing](#nocreepergriefing)
- [noEndermanGriefing](#noendermangriefing)
- [noGhastGriefing](#noghastgriefing)
- [oldFishingLoot](#oldfishingloot)
- [peacefulHunger](#peacefulhunger)
- [playerHeadDrops](#playerheaddrops)
- [reachDistance](#reachdistance)
- [silenceMobs](#silencemobs)
- [silkTouchFarmland](#silktouchfarmland)
- [silkTouchPathBlocks](#silktouchpathblocks)
- [silkTouchSpawners](#silktouchspawners)
- [stonecutterDamage](#stonecutterdamage)
- [strictShulkerShells](#strictshulkershells)
- [zeroTickPlants](#zerotickplants)
- [zombifiedPiglinsSpawningInPortals](#zombifiedpiglinsspawninginportals)

## Implemented Rules

### anvilledBlueIce
Custom amount of packed ice crushed by falling anvils make one blue ice.
- Type: `int`
- Default value: `0`
- Suggested options: `0`, `4`, `9`
- Categories: `FEATURE`, `EXPERIMENTAL`, `SURVIVAL`, `RUG`  
- Additional notes:
  - Value has to be between `0` and `32`
  - From [QuickCarpet](https://github.com/DeadlyMC/QuickCarpet114)

### anvilledIce
Custom amount of frosted ice crushed by falling anvils make one ice. Allows for new type of ice farm.
- Type: `int`
- Default value: `0`
- Suggested options: `0`, `4`, `9`
- Categories: `FEATURE`, `EXPERIMENTAL`, `SURVIVAL`, `RUG`
- Additional notes:
  - Value has to be between `0` and `32`
  - From [QuickCarpet](https://github.com/DeadlyMC/QuickCarpet114)

### anvilledPackedIce
Custom amount of ice crushed by falling anvils make one packed ice.
- Type: `int`
- Default value: `0`
- Suggested options: `0`, `4`, `9`
- Categories: `FEATURE`, `EXPERIMENTAL`, `SURVIVAL`, `RUG`
- Additional notes:
  - Value has to be between `0` and `32`
  - From [QuickCarpet](https://github.com/DeadlyMC/QuickCarpet114)

### cactusFurnaceXP
Amount of XP a Cactus smelted in a furnace gives  
1 XP per Cactus seems to be a bug, as in Bedrock Edition it's only 0.2, which fits more in line with other items
- Type: `double`
- Default value: `1`
- Suggested options: `0.1`, `0.2`, `0.5`, `1`
- Categories: `BUGFIX`, `SURVIVAL`, `RUG`
- Additional notes:
  - Value has to be between `0` and `1`

### concreteConvertOnCauldron
Concrete powder converts to concrete blocks when on top of a filled cauldron
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `FEATURE`, `SURVIVAL`, `RUG`

### dragonDropsElytra
Ender Dragon drops an Elytra when killed
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `FEATURE`, `SURVIVAL`, `RUG`
- Additional notes:
  - Idea from [VanillaTweaks](https://vanillatweaks.net/picker/datapacks/)

### easyHarvesting
Right clicking on fully grown crops harvests and immediately replants it  
Works on: Wheat, Potatoes, Carrots, Beetroots, Nether Warts and Cocoa Beans
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `RUG`

### easyHarvestingRequireHoe
The easyHarvesting feature requires the player to hold a hoe in his main hand
- Type: `boolean`
- Default value: `true`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `RUG`
- Additional notes:
  - Requires easyHarvesting to be enabled

### edibleGoldIngots
Butter is finally edible. Keep in mind 250g of pure butter are not that healthy
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `BUGFIX`, `FEATURE`, `SURVIVAL`, `CLIENT`, `RUG`
- Additional notes:
  - Works server side only, but eating animation is only rendered if the mod is on the client too

### edibleMagmaCream
Magma Cream is edible and gives 10 seconds of Fire Resistance
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `CLIENT`, `RUG`
- Additional notes:
  - Works server side only, but eating animation is only rendered if the mod is on the client too

### edibleNetheriteScraps
Makes Netherite Scraps edible, because, let's be honest, they kinda look like chocolate
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `BUGFIX`, `FEATURE`, `SURVIVAL`, `CLIENT`, `RUG`
- Additional notes:
  - Works server side only, but eating animation is only rendered if the mod is on the client too

### edibleSlimeBalls
Slime Balls are edible and give Jump Boost and Slowness
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `CLIENT`, `RUG`
- Additional notes:
  - Works server side only, but eating animation is only rendered if the mod is on the client too

### enderPearlDamage
Amount of damage dealt by Ender Pearls
- Type: `int`
- Default value: `5`
- Suggested options: `0`, `2`, `3`, `5`
- Categories: `FEATURE`, `SURVIVAL`, `RUG`
- Additional notes:
  - Value has to be between `0` and `10`

### foodInstantHeal
Food heals hearts not hunger like in the first MC versions and naturalRegeneration is off
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `RUG`
- Additional notes:
  - Recommended using with peacefulHunger

### lilyPadsOnCauldron
Lily Pads can be placed on Cauldrons
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `FEATURE`, `SURVIVAL`, `RUG`

### newShulkerBehavior
Makes shulkers behave like in the current 1.17 snapshots  
Shulkers hit by a shulker bullet have a chance to spawn a new shulker and teleport
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `RUG`

### noCreeperGriefing
Prevents Creepers from destroying blocks
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `SURVIVAL`, `RUG`

### noEndermanGriefing
Prevents Endermen from picking up and placing blocks
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `SURVIVAL`, `RUG`

### noGhastGriefing
Prevents Ghasts from destroying blocks
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `SURVIVAL`, `RUG`

### oldFishingLoot
Reverts the fishing loot to how it was before 1.16
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `SURVIVAL`, `RUG`

### peacefulHunger
Players do not lose any hunger like in peaceful mode
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `RUG`

### playerHeadDrops
Players drop their head when killed by a player
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `FEATURE`, `SURVIVAL`, `RUG`
- Additional notes:
  - Idea from [VanillaTweaks](https://vanillatweaks.net/picker/datapacks/)

### reachDistance
Reach in which you can place and break blocks. Value will be 0.5 higher in creative
- Type: `double`
- Default value: `4.5`
- Suggested options: `0`, `4.5`, `5`, `10`
- Categories: `EXPERIMENTAL`, `CREATIVE`, `CLIENT`, `RUG`
- Additional notes:
  - Mod needed on server and client for this feature to work
  - Value has to be between `0` and `100`

### silenceMobs
Mobs named with 'silence_me' stop making noise
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `FEATURE`, `SURVIVAL`, `RUG`
- Additional notes:
  - Idea from [VanillaTweaks](https://vanillatweaks.net/picker/datapacks/)

### silkTouchFarmland
Mining Farmland with a Silk Touch tool will drop itself
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `RUG`

### silkTouchPathBlocks
Mining Path Blocks with a Silk Touch tool will drop itself
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `RUG`

### silkTouchSpawners
Mining Spawners with a Silk Touch tool will drop itself
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `RUG`

### stonecutterDamage
How much damage Stonecutters deal when stepping on them
- Type: `int`
- Default value: `0`
- Suggested options: `0`, `2`, `3`, `5`
- Categories: `BUGFIX`, `SURVIVAL`, `RUG`
- Additional notes:
  - Value has to be between `0` and `10`

### strictShulkerShells
Shulkers always drop a given amount of shulker shells when killed
- Type: `int`
- Default value: `0`
- Suggested options: `0`, `1`, `2`
- Categories: `FEATURE`, `SURVIVAL`, `RUG`
- Additional notes:
  - Value has to be between `0` and `4`
  - Idea from [VanillaTweaks](https://vanillatweaks.net/picker/datapacks/)

### zeroTickPlants
Brings back the ability to force grow certain plants using 0-ticks
- Type: `boolean`
- Default value: `false`
- Required options: `true`, `false`
- Categories: `EXPERIMENTAL`, `FEATURE`, `SURVIVAL`, `RUG`

### zombifiedPiglinsSpawningInPortals
Allows Zombified Piglins to spawn inside Nether Portals
- Type: `boolean`
- Default value: `true`
- Required options: `true`, `false`
- Categories: `SURVIVAL`, `RUG`

## License

This mod is available under the CC0 license. Feel free to learn from it and incorporate it in your own projects.
