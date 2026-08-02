---
sidebar_position: 1
---

# Rule

---

## PistonBlockChunkLoader
If enabled, when this piston/sticky piston head generates a piston head push/pull event, a load ticket of type "piston_block" is added to the chunk where the piston head block is located at the game tick that created the push/pull event, with a duration of 60gt (3s).
#### In any dimension, a diamond ore can be weakly loaded into a 1x1 lazy chunk above a piston.
#### In any dimension, a redstone ore can be weakly loaded into a 1x1 Active chunk above a piston.
#### If there is bedrock below the netherworld and a redstone torch above the next block, a 1x1 block can be lazy loaded.
#### When there are 3X3 weak loading chunks, the central chunk will become a Active loading chunk
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival`

>This rule can be used as an alternative if you do not want to use the Nether portal Load.

## MergeTNTPro
Merging a large amount of TNT to reduce the lag caused by entities and explosions can significantly reduce mspt

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS`, `Feature`, `Survival`,`TNT`

## PearlTickets<sup>`MC < 1.21.2`</sup>
This mod allows ender pearl entities to selectively load chunks that they are about to pass through, so that pearls fired by the pearl cannon will not be lost due to entering unloaded chunks. It can be used instead of the nether portal loading chain in 1.14+.
This mod has a significant performance improvement over the enderPearlChunkLoading function of @gnembon/carpet-extra mod.  
(When enabled in Minecraft>=1.21.2, it can significantly improve the performance of the Pearl Cannon)

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival`

**Ported from：**
SunnySlopes's [PearlTickets](https://github.com/SunnySlopes/PearlTickets)

## SoundSuppressionRadius<sup>`MC > 1.19.4`</sup>
Controls the monitoring radius of the sound suppressor. You can enter a positive integer. The default value in the original version is 16 grids.The maximum value cannot exceed 64.
* Default Value:  `false`
* Optional Parameters: `8`,`16`,`32`
* Categories: `REMS` , `Feature`

## Commandsetnoisesuppressor<sup>`MC > 1.19.4`</sup>
Enables /setnoisesuppressor command to place a sound suppressor
* Default Value:  `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `CREATIVE`

## ComparatorIgnoresStateUpdatesFromBelow<sup>`MC >= 1.20.2`</sup>
When this option is turned on, the comparator ignores state updates from below.  
Means that opening the trap gate will not destroy the comparator
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature`

## PearlPosVelocity
When the ender pearl loading (PearlTickets) is turned on, the pearl will only show the position of the first gt, and the real position and speed of the pearl cannot be checked. After turning this on, it will be displayed on the public screen.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival`

## Endstonefram
You can build Endstonefram like 1.16,it can make it work
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Experimental`

## ProjectileRaycastLength
Changes the distance of the Raycast. If set to 0, all chunks will be checked to reach the destination.
This reduces lag for fast travel. In 1.12 this value is 200.

* Default Value: `0`
* Optional Parameters: `0`, `200`
* Categories: `REMS` , `Survival`

**Ported from：**[EpsilonSMP](https://github.com/EpsilonSMP/Epsilon-Carpet)

## PortalPearlWarp
You can trigger a supertransmission at certain locations.
Below are the locations of the Hell Gates, all positive or negative.

| Nether portal location (center) | Overworld portal location (center) |
|:-------------------------------:|:----------------------------------:|
|             915,915             |         29999600,29999600          |
|            7324,7324            |          3749942,3749942           |
|           58592,58592           |           468735,468735            |
|          468743,468743          |            58585,58585             |

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature`

## ChestMinecartChunkLoader
A chest minecart can force load a 1x1 chunk for 2 seconds. This is enabled when the chest minecart's name is Load.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature`

## EndGatewayChunkLoader<sup>`MC < 1.21`</sup>
When an entity passes through the End gateway, the target chunk will be loaded for 3 seconds like a nether portal.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival`

## ScheduledRandomTickPlants

The planned tick event can trigger the random tick growth behavior of all the following plants, which is used to restore the forced ripening feature of version 1.15.

Cactus, bamboo, chorus flower, sugar cane, kelp, twisting vines, weeping vines

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature`,`Survival`

**Ported from：**[OhMyVanillaMinecraft](https://github.com/hit-mc/OhMyVanillaMinecraft)

## KeepWorldTickUpdate

Minecraft will stop updating entities after 300 ticks of no players in the server's current dimension. This rule will bypass this limitation.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature`

## DisableBatCanSpawn
Stop bats from spawning naturally

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature`

## CactusWrenchSound
Play 'BLOCK_DISPENSER_LAUNCH' sound effect when using the Cactus Wrench.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival` ,`Creative`

## DisablePortalUpdate
Nether portal blocks do not react to block updates.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival` ,`Experimental`

## StringDupeReintroduced<sup>`MC > 1.21.2`</sup>
Reintroduced the line-stirring feature, and you can continue to use the line-stirring machine through this rule.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival` ,`Experimental`

## SharedVillagerDiscounts
The discount obtained by players who cure zombie villagers into villagers will be shared by all players.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival`,`Feature`

## SignCommand
The player right-clicks the sign to execute the command on the sign.The sign starts with /  
(only say tick and player are allowed)

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival`

## SignAllowedCommands
Set a list of allowed commands on the sign, separated by commas, for example: say, tick, player
* Default Value: `false`
* Optional Parameters:`false`, `say`, `player,tick`, `say,player,tick`
* Categories: `REMS` , `Survival`

## Enderpearlloadchunk
This ender pearl loading is ported from 1.21.2. Very useful.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `FEATURE`
  
**Ported from：**[PearlChunkLoading](https://github.com/Crystal0404/PearlChunkLoading)

## Pearltime
This rule controls how many gts the pearl will be destroyed after it exceeds 20m/gt.

* Default Value: `40`
* Optional Parameters: `40`, `0`
* Categories: `REMS` , `FEATURE`


## ItemShadowing
Reintroduced the logic of swapping between inventory slots in 1.16.5.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Experimental`

**Ported from：**[CrystalCarpetAddition](https://github.com/Crystal0404/CrystalCarpetAddition)

## Blockentityreplacement<sup>`MC >= 1.20.2`</sup>
Allows saving and replacing of block entities, used for creating CCE and IAE.

* Default Value: `false`
* Optional Parameters:  `true`, `false`
* Categories: `REMS` , `ExperimentalL`

## Reloadrefreshirongolem
You can build a heavy iron spawner in the end like in 1.14, this rule will make it work
* Default Value:  `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `survival`

## Pre21ThrowableEntityMovement<sup>`MC >= 1.21.2`</sup>
Restored the order of projectile movement from 1.21.2, you can use EnderPearl Cannon like in 1.21.2-
* Default Value: `false`
* Optional Parameters:`true`, `false`
* Categories: `REMS` , `Feature`

## Fixedpearlloading<sup>`MC >= 1.21.2`</sup>
Fixed an issue where ender pearls would unload at high speeds due to being unable to load the current chunk.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `bugfix`

## WanderingTraderNoDisappear
Wandering Trader will no disappear customName is Load
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `feature`

## Pearlnotloadingchunk
Enderpearl no load any chunk
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `feature`

## DurableItemShadow
The item Shadow do not disappear after restarting.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `feature`

## IntroduceHighVersionThrowableEntityMovement<sup>`MC < 1.21.2`</sup>
Introducing projectile motion logic from version 1.21.2+.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `feature`

## NoSensationPearlLoad
When the speed is greater than 300 and it is the first time, a small number of raycast calls will be made. The calculations are saved and the stuttering is reduced on the next call.

* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `feature`

## DisableAIEntitities
Set a list of entities to remove from any AI, separated by commas, for example: zombie,piglin  
For details on disabling AI categories, please refer to DisableAiGoals.
* Default Value: `false`
* Optional Parameters: `false`, `zombie`, `creeper`, `zombie,skeleton`
* Categories: `REMS` , `feature`

## DisableAiGoals
Select the AI function you want to delete, such as: move, attack, look.  
Using the nameplate to name the above function allows you to delete a specific AI instance of an individual entity.
* Default Value:`false`
* Optional Parameters: `false`, `move`, `attack`, `move,attack,look`, `breed,tempt,pickup,work`, `all`
* Categories: `REMS` , `feature`

## Stridergodie
Strider cannot be generated in Hell difficulty above level 170.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Survival`

## FlushFakePlayerNetworkQueue
Every minute, the backlog of outbound packets in the underlying EmbeddedChannel of the fake player is cleared to free up heap memory.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Bugfix`

## DispenserSpearCharge<sup>`MC >= 1.21.11`</sup>
Dispensers can use spears to attack entities in front of them.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Experimental`

## AllowTripwirePlatformDeletion
Players can use the tripwire's abnormal state to interrupt the spawn of the End Obsidian spawn platform, thereby deleting the platform.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `feature`

## CommandBlockWhitelist
The command block whitelist can be enabled or disabled through the backend, preventing certain people with operation privileges from misusing command blocks.
* Open Method: `/cbwhitelist open`
* Close Method: `/cbwhitelist close`
* How to add to the whitelist: `/cbwhitelist add XXX`
* How to remove from the whitelist: `/cbwhitelist remove XXX`

## ReintroduceDolphinPortalItemDupe
Reintroduce the dolphin portal item duplication bug that was fixed in 20w45a.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature`

## FragileBlocks
Set a list of blocks that can be broken quickly, separated by commas, e.g.: obsidian,vault.
* Default Value: `false`
* Optional Parameters: `false`, `obsidian`, `obsidian,vault`...
* Categories: `REMS` , `Feature`

## FixMiningFatigue
Fixes Mining Fatigue III/IV multipliers: III 0.0027→0.027, IV 0.00081→0.0081.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `bugfix`

## RevertZombieFeatures
Reverts two Mojang zombie changes: reinforcements always spawn regular zombies (24w33a), pigmen never spawn with golden spears (1.21.11).
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature`

## NoCreativePickupWhenFull
In creative mode, don't pick up items if inventory has no empty slot and can't stack with existing items.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature` , `Survival`

## NoAnimalGenerationInNewChunks
Prevents animals from spawning naturally during chunk generation.
* Default Value: `false`
* Optional Parameters: `true`, `false`
* Categories: `REMS` , `Feature`

## CommandpetOwnerTransfer
Allows using `/petTransfer <petUUID> <target>` to transfer tamed pet ownership.
* Default Value: `false`
* Optional Parameters: `true`, `ops`, `false`
* Categories: `REMS` , `Survival` , `Command`

---
