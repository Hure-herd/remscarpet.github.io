---
sidebar_position: 1
---

# 规则

---

## 清理假玩家网络队列(FlushFakePlayerNetworkQueue)
每分钟清空假玩家底层EmbeddedChannel中积压的出站数据包以释放堆内存
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Bugfix`

## 投掷物Raycast长度(ProjectileRaycastLength)
更改Raycast的距离。如果设置为0，将检查所有到达目的地的块。  
这减少了快速移动的延迟。在1.12中该值为200。
* 默认值: `0`
* 可选参数: `0`, `200`
* 分类: `REMS` , `Survival`

**移植自：**[EpsilonSMP](https://github.com/EpsilonSMP/Epsilon-Carpet)

## 箱子矿车加载区块(ChestMinecartChunkLoader)
箱子矿车可以强加载1x1的区块持续2s,当箱子矿车的名字是Load时生效。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 流商不消失(WanderingTraderNoDisappear)
名字是Load的流浪商人不会消失
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `feature`

## 珍珠超传(PortalPearlWarp)
可以在某些特定的位置触发超传。  
下面是地狱门的位置，都是正正或者负负

| 地狱传送门位置（正中央)  |   主世界传送门位置（正中央)    |
|:-------------:|:------------------:|
|    915,915    | 29999600,29999600  |
|   7324,7324   |  3749942,3749942   |
|  58592,58592  |   468735,468735    |
| 468743,468743 |   58585,58585      |
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 活塞头加载(PistonBlockChunkLoader)
开启后，当该活塞/黏性活塞头产生活塞头的推出/拉回事件时，在创建推出/拉回事件的那一游戏刻为**活塞头方块所在区块**添加类型为"piston_block"的加载票，持续时间为60gt（3s）。
#### 在任何维度，活塞上方有钻石矿时可以弱加载1x1的区块
#### 在任何维度，活塞上方有红石矿时可以强加载1x1的区块
#### 在地狱下方有基岩，后一格上方是红石火把时可以弱加载1x1的区块
#### 当有3X3的弱加载区块的时候，最中心的区块会变成强加载区块
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival`
> 如果不想使用地狱门加载链的话，此规则可作为替代方案。

## 炽足兽去死(Stridergodie)
让炽足兽在地狱170高以上无法生成
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival`

## 保持实体更新(KeepWorldTickUpdate)
在服务器当前维度没有玩家的300tick后，Minecraft会停止实体相关的更新，这条规则会绕过这个限制。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 计划刻催熟植物(ScheduledRandomTickPlants)
可以让计划刻事件触发以下所有植物的随机刻生长行为，用于恢复1.15版本的强制催熟特性。  
仙人掌、竹子、紫颂花、甘蔗、海带、缠怨藤、垂泪藤
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`,`Survival`


**移植自：**[OhMyVanillaMinecraft](https://github.com/hit-mc/OhMyVanillaMinecraft)

## 更好的TNT合并(MergeTNTPro)
合并大量TNT以减小实体及爆炸带来的卡顿，能显著降低mspt

* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS`, `Feature`, `Survival`,`TNT`

## 激进的合并TNT(MergeTNTMax)
更加激进的TNT合并，卡顿相较于Pro更低

* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS`, `Feature`, `Survival`,`TNT`

## 禁止蝙蝠生成(DisableBatCanSpawn)
阻止蝙蝠自然生成
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 仙人掌扳手音效(CactusWrenchSound)
使用仙人掌扳手时播放 'BLOCK_DISPENSER_LAUNCH' 音效
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival` ,`Creative`

## 禁止传送门更新(DisablePortalUpdate)
下界传送门方块收到方块更新后不会做出反应
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival` ,`Experimental`

## 末地折跃门加载(EndGatewayChunkLoader)<sup>`MC < 1.21`</sup>
当实体穿越末路之地折跃门时，目标区块会像下界传送门一样使目标区块获得3s的加载。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival`

## 物品分身(ItemShadowing)
重新引入1.16.5物品栏之间交换的逻辑
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Experimental`

**移植自：**[CrystalCarpetAddition](https://github.com/Crystal0404/CrystalCarpetAddition)

## 共享打折(SharedVillagerDiscounts)
玩家将僵尸村民治疗为村民后的获得的折扣将共享给所有玩家
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival`,`Feature`

## 末地石农场(Endstonefram)
你可以像1.16一样建造末地石农场，这个规则可以让他工作
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Experimental`

## 重载式刷铁机(Reloadrefreshirongolem)
你可以像1.14一样在末地建造重载式刷铁机，这个规则可以让他工作
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `survival`

## 重新引入POI传送(TeleportToPoiWithoutPortals)
重新添加传送至没有传送门方块的传送门POI的规则
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Experimental`

## 命令告示牌(SignCommand)
玩家右键单击标牌，执行标牌上的命令  
在告示牌以/开头（只允许say tick和player）
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival`

## 重新引入羊驼复制(ReintroduceLlamaItemDuplicating)
重新引入1.14-1.15的羊驼物品复制。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 重新引入海豚过门物品复制(ReintroduceDolphinPortalItemDupe)
重新引入20w45a修复的海豚携带物品穿越传送门时的物品复制。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 新区块不生成动物(NoAnimalGenerationInNewChunks)
禁止在区块生成时自然生成动物（牛羊猪鸡等）。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 修复挖掘疲劳倍率(FixMiningFatigue)
修复挖掘疲劳 III/IV 级的挖掘速度倍率：III 0.0027→0.027, IV 0.00081→0.0081。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `bugfix`

## 创造模式背包满时禁止拾取(NoCreativePickupWhenFull)
创造模式下若背包无空位且无法与已有物品堆叠，则不会拾起物品。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature` , `Survival`

## 宠物主人转让(CommandpetOwnerTransfer)
允许使用 `/petTransfer <宠物UUID> <目标玩家>` 命令将已驯服宠物转让给其他玩家。
* 默认值: `false`
* 可选参数: `true`, `ops`, `false`
* 分类: `REMS` , `Survival` , `Command`

## 生存模式OP编辑命令方块(OpInSurvivalCommandBlocks)
允许 OP 在生存模式下编辑命令方块
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 声音抑制器范围控制(SoundSuppressionRadius)
控制声音抑制器的监听范围半径，可输入一个正整数，原版默认为16格，最大不能超过64
* 默认值: `false`
* 可选参数: `8`,`16`,`32`
* 分类: `REMS` , `Feature`

## 末影珍珠加载(PearlTickets)<sup>`MC < 1.21.2, REMS ≤ V1.3.11`</sup>
> **已在 V1.3.12 移除。** 此规则仅存在于 REMS-Carpet-Addition **V1.3.11 及更早版本**，且仅限 Minecraft < 1.21.2。已被 `Enderpearlloadchunk` + `Pearltime` + `Fixedpearlloading`取代。

这个规则允许末影珍珠实体选择性地加载即将通过的区块，这样珍珠炮打出的珍珠就不会因为进入未加载区块而丢失。在1.14+中可以替代地狱门加载链使用。   
该mod相比于@gnembon/carpet-extra mod的enderPearlChunkLoading功能有显著的性能提升。  
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival`

## 末影真实位置(PearlPosVelocity)<sup>`MC < 1.21.2, REMS ≤ V1.3.11`</sup>
> **已在 V1.3.12 移除。** 此规则仅存在于 REMS-Carpet-Addition **V1.3.11 及更早版本**，且仅限 Minecraft < 1.21.2。已被 `Enderpearlloadchunk` + `Pearltime` + `Fixedpearlloading`取代。

在开启末影珍珠加载(PearlTickets)的时候，珍珠只会显示第一gt的位置，查看不到珍珠的真实位置和速度，开启这个后，会在公屏显示出来。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival`

**移植自：**
SunnySlopes 的[PearlTickets](https://github.com/SunnySlopes/PearlTickets)

## 珍珠加载时间(Pearltime)<sup>`MC < 1.21.2`</sup>
这个规则可以控制珍珠在大于20m/gt后多少gt被销毁
* 默认值: `40`
* 可选参数: `40`, `0`
* 分类: `REMS` , `FEATURE`

## 末影珍珠加载(Enderpearlloadchunk)<sup>`MC < 1.21.2`</sup>
这个末影珍珠加载是从1.21.2移植下来的。十分好用
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `FEATURE`

**移植自：**[PearlChunkLoading](https://github.com/Crystal0404/PearlChunkLoading)

## 持久物品分身(DurableItemShadow)
重启后物品分身不消失
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `feature`

## 清除已保存珍珠轨迹命令开关(CommandClearPearTrail)
启用 /clearPearlTrail 命令以清除已保存的 PearlTrail
* 默认值: `ops`
* 可选参数: `ops`, `true`, `flase`
* 分类: `REMS` , `Creative`, `Command`

## 放置声音抑制器命令开关(Commandsetnoisesuppressor)
启用/setnoisesuppressor命令来放置声音抑制器
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `CREATIVE`

## 比较器忽略来自下方的状态更新(ComparatorIgnoresStateUpdatesFromBelow)<sup>`MC > 1.20.1`</sup>

比较器会忽略来自下方的状态更新,意味着开启活板门不会破坏比较器
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 重新引入拌线骗特性(StringDupeReintroduced)<sup>`MC > 1.21.1`</sup>
重新引入拌线骗特性，可以通过此规则来继续使用刷线机
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival` ,`Experimental`

## 恢复1.21.2-的投掷物移动顺序(Pre21ThrowableEntityMovement)<sup>`MC >= 1.21.2`</sup>
恢复1.21.2-的投掷物移动顺序,你可以使用1.21.2-的珍珠炮
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 珍珠不加载(Pearlnotloadingchunk)<sup>`MC >= 1.21.2`</sup>
珍珠不加载任何区块
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `feature`

## 引入高版本投掷物运动(IntroduceHighVersionThrowableEntityMovement)<sup>`MC < 1.21.2`</sup>
引入1.21.2+版本的投掷物运动逻辑
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `feature`

## 修复珍珠加载(Fixedpearlloading)
修复了在高速下，末影珍珠会因为无法加载当前区块而卸载
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `bugfix`

## 方块实体替换(Blockentityreplacement)<sup>`MC > 1.20.1`</sup>
允许方块实体的保存和替换，用于制作CCE和IAE
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `ExperimentalL`

## 无感珍珠加载(NoSensationPearlLoad)
在大于300速度且第一次时会少量调用raycast，计算后保存，下一次调用时直接去除raycast
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `feature`

## 告示牌允许指令列表(SignAllowedCommands)
设置在告示牌上允许使用的指令的列表，使用逗号分隔，例如: say,tick,player
* 默认值: `false`
* 可选参数: `false`, `say`, `player,tick`, `say,player,tick`
* 分类: `REMS` , `Survival`

## 禁用AI的实体类型(DisableAIEntitities)
设置移除任意AI的实体列表，使用逗号分隔，例如: zombie,piglin  
禁用AI的类别类别详细请看DisableAiGoals
* 默认值: `false`
* 可选参数: `false`, `zombie`, `creeper`, `zombie,skeleton`
* 分类: `REMS` , `feature`

## 禁用AI的类别(DisableAiGoals)
选择要删除的 AI 功能 如: move, attack, look  
使用命名牌命名为上方功能后可以删除单独实体的某个AI
* 默认值: `false`
* 可选参数: `false`, `move`, `attack`, `move,attack,look`, `breed,tempt,pickup,work`, `all`
* 分类: `REMS` , `feature`

## 易碎方块(FragileBlocks)
"设置可以被快速破坏的方块列表，使用逗号分隔，例如: obsidian,vault"。
* 默认值: `false`
* 可选参数: `false`, `obsidian`, `obsidian,vault`...
* 分类: `REMS` , `Feature`

## 回退僵尸特性(RevertZombieFeatures)
回退Mojang的两个僵尸更改：增援始终为普通僵尸（24w33a前行为），猪人不再生成金矛（1.21.11前行为）。
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Feature`

## 发射器可以发射矛(DispenserSpearCharge)<sup>`MC > 1.21.8`</sup>
发射器可以使用长矛攻击面前的实体
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Experimental`

## 引入绊线删除平台(AllowTripwirePlatformDeletion)<sup>`MC >= 1.20.6`</sup>
允许玩家利用绊线的异常状态来中断末地黑曜石出生平台的生成，从而删除平台
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `feature`

## 虚空交易(VoidTrading)<sup>`MC >= 1.20.6`</sup>
恢复虚空交易，使用 /noEndGatewayTicket 命令取消某位置的折跃门的加载
* 默认值: `false`
* 可选参数: `true`, `false`
* 分类: `REMS` , `Survival`

## 取消折跃门加载命令开关(CommandnoEndGatewayTicket)<sup>`MC >= 1.20.6`</sup>
启用 /noEndGatewayTicket 命令来取消某位置的折跃门的加载
* 默认值: `ops`
* 可选参数: `ops`, `true`, `flase`
* 分类: `REMS` , `Creative`, `Command`

## 命令方块白名单(CommandBlockWhitelist)
通过后台可以开启与关闭命令方块白名单，禁止某些存在拥有op的人乱使用命令方块。
* 开启方法: `/cbwhitelist open`
* 关闭方法: `/cbwhitelist close`
* 添加白名单方法: `/cbwhitelist add XXX`
* 删除白名单方法: `/cbwhitelist remove XXX`

---
