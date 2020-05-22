# MCPlayerEntity #MC玩家实体

这个类由mod-id为`crafttweaker`的模组添加. 因此，如果要使用此功能，则需要安装此mod。

## 导入类
如果遇到任何问题（例如强制转换数组），则可能需要导入软件包，因此，最好的方式就是导入包支持。
```zenscript
crafttweaker.api.entity.player.MCPlayerEntity
```

## 使用方式
### addExhaustion #增加饥饿值

通过所提供的数值增加饥饿值

```zenscript
myMCPlayerEntity.addExhaustion(exhaustion as float);
```

| 参数         | 类型          | 描述    |
| ---------- | ----------- | ----- |
| exhaustion | 浮点数据[float] | 未提供说明 |


### addExperienceLevel #提升经验等级

提升此玩家的经验等级

```zenscript
myMCPlayerEntity.addExperienceLevel(levels as int);
```

| 参数     | 类型      | 说明    |
| ------ | ------- | ----- |
| levels | int #整型 | 未提供说明 |


### addItemStackToInventory #在背包中添加物品堆叠

返回为布尔值

```zenscript
myMCPlayerEntity.addItemStackToInventory(p_191521_1_ as crafttweaker.api.item.IItemStack);
```

| 参数            | 返回值类型                                                             | 描述    |
| ------------- | ----------------------------------------------------------------- | ----- |
| p_191521_1_ | [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack) | 未提供说明 |


### addMovementStat #添加移动统计

为移动统计添加一个值——如跑步、步行、游泳或攀登。

```zenscript
myMCPlayerEntity.addMovementStat(p_71000_1_ as double, p_71000_3_ as double, p_71000_5_ as double);
```

| 参数           | 返回值类型       | 描述    |
| ------------ | ----------- | ----- |
| p_71000_1_ | double #双精度 | 未提供说明 |
| p_71000_3_ | double #双精度 | 未提供说明 |
| p_71000_5_ | double #双精度 | 未提供说明 |


### addPotionEffect #添加药水效果

返回为布尔值

```zenscript
myMCPlayerEntity.addPotionEffect(effectInstanceIn as crafttweaker.api.potion.MCPotionEffectInstance);
```

| 参数                     | 返回值类型                                                                                         | 描述    |
| ---------------------- | --------------------------------------------------------------------------------------------- | ----- |
| effectInstanceIn #效果实例 | [crafttweaker.api.potion.MCPotionEffectInstance](/vanilla/api/potions/MCPotionEffectInstance) | 未提供说明 |


### addScore #添加分数

添加到玩家分数

```zenscript
myMCPlayerEntity.addScore(scoreIn as int);
```

| 参数      | 返回值类型   | 描述    |
| ------- | ------- | ----- |
| scoreIn | int #整型 | 未提供说明 |


### addTag #添加tag

返回为布尔值

```zenscript
myMCPlayerEntity.addTag(tag as String);
```

| 参数      | 返回值类型       | 描述    |
| ------- | ----------- | ----- |
| tag #标签 | 字符串[string] | 未提供说明 |


### addVelocity #增加速度

为实体的当前速度添加一个值,并设置为true

```zenscript
myMCPlayerEntity.addVelocity(x as double, y as double, z as double);
```

| 参数 | 返回值类型       | 描述    |
| -- | ----------- | ----- |
| x  | double #双精度 | 未提供说明 |
| y  | double #双精度 | 未提供说明 |
| z  | double #双精度 | 未提供说明 |


### allowLogging #允许记录日志

返回为布尔值

```zenscript
myMCPlayerEntity.allowLogging();
```

### attackable #可攻击的

返回为布尔值

```zenscript
myMCPlayerEntity.attackable();
```

### attemptTeleport #是否尝试传送

返回为布尔值

```zenscript
myMCPlayerEntity.attemptTeleport(p_213373_1_ as double, p_213373_3_ as double, p_213373_5_ as double, p_213373_7_ as boolean);
```

| 参数            | 返回值类型       | 描述    |
| ------------- | ----------- | ----- |
| p_213373_1_ | double #双精度 | 未提供说明 |
| p_213373_3_ | double #双精度 | 未提供说明 |
| p_213373_5_ | double #双精度 | 未提供说明 |
| p_213373_7_ | 布尔值         | 未提供说明 |


### baseTick #基础游戏刻

Gets called every tick from main Entity class #从主要实体类获取所有游戏刻

```zenscript
myMCPlayerEntity.baseTick();
```

### canAttackPlayer #可以攻击玩家

返回为布尔值

```zenscript
myMCPlayerEntity.canAttackPlayer(other as crafttweaker.api.entity.player.MCPlayerEntity);
```

| 参数    | 返回值类型                                                                                      | 描述    |
| ----- | ------------------------------------------------------------------------------------------ | ----- |
| other | [crafttweaker.api.entity.player.MCPlayerEntity](/vanilla/api/entity/player/MCPlayerEntity) | 未提供说明 |


### canBeAttackedWithItem #可以被物体攻击

如果可能用物品攻击该实体,则返回true

返回为布尔值

```zenscript
myMCPlayerEntity.canBeAttackedWithItem();
```

### canBeCollidedWith #具有碰撞箱

如果此实体可以阻止其他实体的移动,则反为真

返回为布尔值

```zenscript
myMCPlayerEntity.canBeCollidedWith();
```

### canBeHitWithPotion #可以被药水瓶击中

如果实体为盔甲架,则返回false 如果是其他实体生物则返回为true

返回为布尔值

```zenscript
myMCPlayerEntity.canBeHitWithPotion();
```

### canBePushed #可以被推动

如果该实体在与其他实体碰撞时可以被推动,则返回值true

返回为布尔值

```zenscript
myMCPlayerEntity.canBePushed();
```

### canBeRiddenInWater #可以潜水

返回为布尔值

```zenscript
myMCPlayerEntity.canBeRiddenInWater();
```

### canBreatheUnderwater #可以水下呼吸

返回为布尔值

```zenscript
myMCPlayerEntity.canBreatheUnderwater();
```

### canEat #可以进食

返回为布尔值

```zenscript
myMCPlayerEntity.canEat(ignoreHunger as boolean);
```

| 参数           | 返回值类型 | 描述    |
| ------------ | ----- | ----- |
| ignoreHunger | 布尔值   | 未提供说明 |


### canHarvestBlock #可以破坏方块

返回为布尔值

```zenscript
myMCPlayerEntity.canHarvestBlock(state as crafttweaker.api.block.MCBlockState);
```

| 参数    | 返回值类型                                                                   | 描述    |
| ----- | ----------------------------------------------------------------------- | ----- |
| state | [crafttweaker.api.block.MCBlockState](/vanilla/api/blocks/MCBlockState) | 未提供说明 |


### canPassengerSteer #可以乘坐

返回为布尔值

```zenscript
myMCPlayerEntity.canPassengerSteer();
```

### canPlayerEdit #可以由玩家编辑

返回此玩家是否可以在某个地点使用给定的堆栈修改方块。 <p> 查询位置是 {@code pos.offset(facing.getOpposite()}。 返回：`此玩家是否可以修改当前世界中查询的位置` @see ItemStack#canPlaceOn(Block) @see ItemStack#canEditBlocks() @see PlayerCapabilities#allowededge

返回为布尔值

```zenscript
myMCPlayerEntity.canPlayerEdit(pos as crafttweaker.api.util.BlockPos, facing as crafttweaker.api.util.Direction, stack as crafttweaker.api.item.IItemStack);
```

| 参数 | 类型                                                                | 说明    |
| -- | ----------------------------------------------------------------- | ----- |
| 点  | [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos)      | 未提供说明 |
| 方向 | [crafttweaker.api.util.Direction](/vanilla/api/util/Direction)    | 未提供说明 |
| 堆叠 | [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack) | 未提供说明 |


### canRenderOnFire #是否能被渲染为着火

返回该实体能否被渲染为着火

返回为布尔值

```zenscript
myMCPlayerEntity.canRenderOnFire();
```

### canRiderInteract #是否可以互动

返回为布尔值

```zenscript
myMCPlayerEntity.canRiderInteract();
```

### canSwim #是否可以游泳

返回为布尔值

```zenscript
myMCPlayerEntity.canSwim();
```

### canTrample #是否能被踩踏

返回为布尔值

```zenscript
myMCPlayerEntity.canTrample(state as crafttweaker.api.block.MCBlockState, pos as crafttweaker.api.util.BlockPos, fallDistance as float);
```

| 参数   | 类型                                                                      | 说明    |
| ---- | ----------------------------------------------------------------------- | ----- |
| 状态   | [crafttweaker.api.block.MCBlockState](/vanilla/api/blocks/MCBlockState) | 未提供说明 |
| 点    | [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos)            | 未提供说明 |
| 下落距离 | 浮点                                                                      | 未提供说明 |


### canUpdate #是否能被更新

返回为布尔值

```zenscript
myMCPlayerEntity.canUpdate();
```


```zenscript
myMCPlayerEntity.canUpdate(值为布尔型);
```

| 参数 | 类型  | 说明    |
| -- | --- | ----- |
| 值  | 布尔值 | 未提供说明 |


### canUseCommandBlock #是否可以使用命令方块

返回为布尔值

```zenscript
myMCPlayerEntity.canUseCommandBlock();
```

### clearActivePotions #清除药水效果

返回为布尔值

```zenscript
myMCPlayerEntity.clearActivePotions();
```

### clearBedPosition #清除床的位置

```zenscript
myMCPlayerEntity.clearBedPosition();
```

### closeScreen #关闭屏幕

把当前合成栏设置回2x2个格子

```zenscript
myMCPlayerEntity.closeScreen();
```

### curePotionEffects #清除药水效果

返回为布尔值

```zenscript
myMCPlayerEntity.curePotionEffects(治疗的效果为 crafttweaker.api.item.IItemStack);
```

| 参数    | 类型                                                                | 说明    |
| ----- | ----------------------------------------------------------------- | ----- |
| 治疗的效果 | [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack) | 未提供说明 |


### detach #分离

```zenscript
myMCPlayerEntity.detach();
```

### disableShield #禁用盾

```zenscript
myMCPlayerEntity.disableShield（p_190777_1_ 为布尔值）；
```

| Parameter     | Type    | Description             |
| ------------- | ------- | ----------------------- |
| p_190777_1_ | boolean | No description provided |


### doesEntityNotTriggerPressurePlate

Return whether this entity should NOT trigger a pressure plate or a tripwire.

Returns boolean

```zenscript
myMCPlayerEntity.doesEntityNotTriggerPressurePlate();
```

### equals

Returns boolean

```zenscript
myMCPlayerEntity.equals(p_equals_1_ as Object);
```

| Parameter     | Type   | Description             |
| ------------- | ------ | ----------------------- |
| p_equals_1_ | Object | No description provided |


### extinguish

Removes fire from entity.

```zenscript
myMCPlayerEntity.extinguish();
```

### fall

```zenscript
myMCPlayerEntity.fall(distance as float, damageMultiplier as float);
```

| Parameter        | Type  | Description             |
| ---------------- | ----- | ----------------------- |
| distance         | float | No description provided |
| damageMultiplier | float | No description provided |


### findAmmo

Returns [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack)

```zenscript
myMCPlayerEntity.findAmmo(shootable as crafttweaker.api.item.IItemStack);
```

| Parameter | Type                                                              | Description             |
| --------- | ----------------------------------------------------------------- | ----------------------- |
| shootable | [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack) | No description provided |


### func_213300_bk

Returns boolean

```zenscript
myMCPlayerEntity.func_213300_bk();
```

### func_213312_b

```zenscript
myMCPlayerEntity.func_213312_b(p_213312_1_ as double, p_213312_3_ as double, p_213312_5_ as double);
```

| Parameter     | Type   | Description             |
| ------------- | ------ | ----------------------- |
| p_213312_1_ | double | No description provided |
| p_213312_3_ | double | No description provided |
| p_213312_5_ | double | No description provided |


### func_213314_bj

Returns boolean

```zenscript
myMCPlayerEntity.func_213314_bj();
```

### func_213343_cS

Returns float

```zenscript
myMCPlayerEntity.func_213343_cS();
```

### func_213365_e

Returns boolean

```zenscript
myMCPlayerEntity.func_213365_e(itemstackIn as crafttweaker.api.item.IItemStack);
```

| Parameter   | Type                                                              | Description             |
| ----------- | ----------------------------------------------------------------- | ----------------------- |
| itemstackIn | [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack) | No description provided |


### getAIMoveSpeed

the movespeed used for the new AI system

Returns float

```zenscript
myMCPlayerEntity.getAIMoveSpeed();
```

### getAbsorptionAmount

Returns the amount of health added by the Absorption effect.

Returns float

```zenscript
myMCPlayerEntity.getAbsorptionAmount();
```

### getActiveItemStack

Returns [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack)

```zenscript
myMCPlayerEntity.getActiveItemStack();
```

### getActivePotionEffect

returns the PotionEffect for the supplied Potion if it is active, null otherwise.

Returns [crafttweaker.api.potion.MCPotionEffectInstance](/vanilla/api/potions/MCPotionEffectInstance)

```zenscript
myMCPlayerEntity.getActivePotionEffect(potionIn as crafttweaker.api.potion.MCPotionEffect);
```

| Parameter | Type                                                                          | Description             |
| --------- | ----------------------------------------------------------------------------- | ----------------------- |
| potionIn  | [crafttweaker.api.potion.MCPotionEffect](/vanilla/api/potions/MCPotionEffect) | No description provided |


### getActivePotionEffects

Returns Collection<[crafttweaker.api.potion.MCPotionEffectInstance](/vanilla/api/potions/MCPotionEffectInstance)>

```zenscript
myMCPlayerEntity.getActivePotionEffects();
```

### getAdjustedHorizontalFacing

Gets the horizontal facing direction of this Entity, adjusted to take specially-treated entity types into account.

Returns [crafttweaker.api.util.Direction](/vanilla/api/util/Direction)

```zenscript
myMCPlayerEntity.getAdjustedHorizontalFacing();
```

### getAir

Returns int

```zenscript
myMCPlayerEntity.getAir();
```

### getAlwaysRenderNameTagForRender

Returns boolean

```zenscript
myMCPlayerEntity.getAlwaysRenderNameTagForRender();
```

### getArrowCountInEntity

Returns int

```zenscript
myMCPlayerEntity.getArrowCountInEntity();
```

### getBedDirection

gets the Direction for the camera if this entity is sleeping

Returns [crafttweaker.api.util.Direction](/vanilla/api/util/Direction)

```zenscript
myMCPlayerEntity.getBedDirection();
```

### getBedLocation

Returns [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos)

```zenscript
myMCPlayerEntity.getBedLocation();
```

### getBlockState

Returns [crafttweaker.api.block.MCBlockState](/vanilla/api/blocks/MCBlockState)

```zenscript
myMCPlayerEntity.getBlockState();
```

### getBrightness

Gets how bright this entity is.

Returns float

```zenscript
myMCPlayerEntity.getBrightness();
```

### getBrightnessForRender

Returns int

```zenscript
myMCPlayerEntity.getBrightnessForRender();
```

### getCachedUniqueIdString

Returns String

```zenscript
myMCPlayerEntity.getCachedUniqueIdString();
```

### getClassification

Returns [crafttweaker.api.entity.MCEntityClassification](/vanilla/api/entities/MCEntityClassification)

```zenscript
myMCPlayerEntity.getClassification(forSpawnCount as boolean);
```

| Parameter     | Type    | Description             |
| ------------- | ------- | ----------------------- |
| forSpawnCount | boolean | No description provided |


### getCollisionBorderSize

Returns float

```zenscript
myMCPlayerEntity.getCollisionBorderSize();
```

### getCooldownPeriod

Returns float

```zenscript
myMCPlayerEntity.getCooldownPeriod();
```

### getCooledAttackStrength

Returns the percentage of attack power available based on the cooldown (zero to one).

Returns float

```zenscript
myMCPlayerEntity.getCooledAttackStrength(adjustTicks as float);
```

| Parameter   | Type  | Description             |
| ----------- | ----- | ----------------------- |
| adjustTicks | float | No description provided |


### getDigSpeed

Returns float

```zenscript
myMCPlayerEntity.getDigSpeed(state as crafttweaker.api.block.MCBlockState);
```

| Parameter | Type                                                                    | Description             |
| --------- | ----------------------------------------------------------------------- | ----------------------- |
| state     | [crafttweaker.api.block.MCBlockState](/vanilla/api/blocks/MCBlockState) | No description provided |



Returns float

```zenscript
myMCPlayerEntity.getDigSpeed(arg0 as crafttweaker.api.block.MCBlockState, arg1 as crafttweaker.api.util.BlockPos);
```

| Parameter | Type                                                                    | Description             |
| --------- | ----------------------------------------------------------------------- | ----------------------- |
| arg0      | [crafttweaker.api.block.MCBlockState](/vanilla/api/blocks/MCBlockState) | No description provided |
| arg1      | [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos)            | No description provided |


### getDistanceSq

Returns double

```zenscript
myMCPlayerEntity.getDistanceSq(x as double, y as double, z as double);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| x         | double | No description provided |
| y         | double | No description provided |
| z         | double | No description provided |


### getEntityId

Returns int

```zenscript
myMCPlayerEntity.getEntityId();
```

### getEntityString

Returns String

```zenscript
myMCPlayerEntity.getEntityString();
```

### getEyeHeight

Returns float

```zenscript
myMCPlayerEntity.getEyeHeight();
```

### getFireTimer

Returns int

```zenscript
myMCPlayerEntity.getFireTimer();
```

### getHealth

Returns float

```zenscript
myMCPlayerEntity.getHealth();
```

### getHeight

Returns float

```zenscript
myMCPlayerEntity.getHeight();
```

### getHeldItemMainhand

Returns [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack)

```zenscript
myMCPlayerEntity.getHeldItemMainhand();
```

### getHeldItemOffhand

Returns [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack)

```zenscript
myMCPlayerEntity.getHeldItemOffhand();
```

### getHorizontalFacing

Gets the horizontal facing direction of this Entity.

Returns [crafttweaker.api.util.Direction](/vanilla/api/util/Direction)

```zenscript
myMCPlayerEntity.getHorizontalFacing();
```

### getIdleTime

Returns int

```zenscript
myMCPlayerEntity.getIdleTime();
```

### getItemInUseCount

Returns int

```zenscript
myMCPlayerEntity.getItemInUseCount();
```

### getItemInUseMaxCount

Returns int

```zenscript
myMCPlayerEntity.getItemInUseMaxCount();
```

### getLastAttackedEntityTime

Returns int

```zenscript
myMCPlayerEntity.getLastAttackedEntityTime();
```

### getLuck

Returns float

```zenscript
myMCPlayerEntity.getLuck();
```

### getMaxAir

Returns int

```zenscript
myMCPlayerEntity.getMaxAir();
```

### getMaxFallHeight

The maximum height from where the entity is alowed to jump (used in pathfinder)

Returns int

```zenscript
myMCPlayerEntity.getMaxFallHeight();
```

### getMaxHealth

Returns float

```zenscript
myMCPlayerEntity.getMaxHealth();
```

### getMaxInPortalTime

Return the amount of time this entity should stay in a portal before being transported.

Returns int

```zenscript
myMCPlayerEntity.getMaxInPortalTime();
```

### getMountedYOffset

Returns the Y offset from the entity's position for any entity riding this one.

Returns double

```zenscript
myMCPlayerEntity.getMountedYOffset();
```

### getPitch

Gets the current pitch of the entity.

Returns float

```zenscript
myMCPlayerEntity.getPitch(partialTicks as float);
```

| Parameter    | Type  | Description             |
| ------------ | ----- | ----------------------- |
| partialTicks | float | No description provided |


### getPortalCooldown

Return the amount of cooldown before this entity can use a portal again.

Returns int

```zenscript
myMCPlayerEntity.getPortalCooldown();
```

### getPosition

Get the position in the world. <b>{@code null} is not allowed!</b> If you are not an entity in the world, return the coordinates 0, 0, 0

Returns [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos)

```zenscript
myMCPlayerEntity.getPosition();
```

### getRenderScale

Returns float

```zenscript
myMCPlayerEntity.getRenderScale();
```

### getRevengeTimer

Returns int

```zenscript
myMCPlayerEntity.getRevengeTimer();
```

### getRotationYawHead

Returns float

```zenscript
myMCPlayerEntity.getRotationYawHead();
```

### getScore

Returns int

```zenscript
myMCPlayerEntity.getScore();
```

### getScoreboardName

Returns a String to use as this entity's name in the scoreboard/entity selector systems

Returns String

```zenscript
myMCPlayerEntity.getScoreboardName();
```

### getSleepTimer

Returns int

```zenscript
myMCPlayerEntity.getSleepTimer();
```

### getSubmergedHeight

Returns double

```zenscript
myMCPlayerEntity.getSubmergedHeight();
```

### getSwimAnimation

Returns float

```zenscript
myMCPlayerEntity.getSwimAnimation(partialTicks as float);
```

| Parameter    | Type  | Description             |
| ------------ | ----- | ----------------------- |
| partialTicks | float | No description provided |


### getSwingProgress

Gets the progression of the swing animation, ranges from 0.0 to 1.0.

Returns float

```zenscript
myMCPlayerEntity.getSwingProgress(partialTickTime as float);
```

| Parameter       | Type  | Description             |
| --------------- | ----- | ----------------------- |
| partialTickTime | float | No description provided |


### getTags

Returns Set<String>

```zenscript
myMCPlayerEntity.getTags();
```

### getTeleportDirection

Returns [crafttweaker.api.util.Direction](/vanilla/api/util/Direction)

```zenscript
myMCPlayerEntity.getTeleportDirection();
```

### getTicksElytraFlying

Returns int

```zenscript
myMCPlayerEntity.getTicksElytraFlying();
```

### getTotalArmorValue

Returns the current armor value as determined by a call to InventoryPlayer.getTotalArmorValue

Returns int

```zenscript
myMCPlayerEntity.getTotalArmorValue();
```

### getWidth

Returns float

```zenscript
myMCPlayerEntity.getWidth();
```

### getXPSeed

Returns int

```zenscript
myMCPlayerEntity.getXPSeed();
```

### getYOffset

Returns the Y Offset of this entity.

Returns double

```zenscript
myMCPlayerEntity.getYOffset();
```

### getYaw

Gets the current yaw of the entity

Returns float

```zenscript
myMCPlayerEntity.getYaw(partialTicks as float);
```

| Parameter    | Type  | Description             |
| ------------ | ----- | ----------------------- |
| partialTicks | float | No description provided |


### giveExperiencePoints

```zenscript
myMCPlayerEntity.giveExperiencePoints(p_195068_1_ as int);
```

| Parameter     | Type | Description             |
| ------------- | ---- | ----------------------- |
| p_195068_1_ | int  | No description provided |


### handleStatusUpdate

```zenscript
myMCPlayerEntity.handleStatusUpdate(id as byte);
```

| Parameter | Type | Description             |
| --------- | ---- | ----------------------- |
| id        | byte | No description provided |


### handleWaterMovement

Returns if this entity is in water and will end up adding the waters velocity to the entity

Returns boolean

```zenscript
myMCPlayerEntity.handleWaterMovement();
```

### hasCustomName

Returns boolean

```zenscript
myMCPlayerEntity.hasCustomName();
```

### hasNoGravity

Returns boolean

```zenscript
myMCPlayerEntity.hasNoGravity();
```

### hasPermissionLevel

Returns boolean

```zenscript
myMCPlayerEntity.hasPermissionLevel(p_211513_1_ as int);
```

| Parameter     | Type | Description             |
| ------------- | ---- | ----------------------- |
| p_211513_1_ | int  | No description provided |


### hasReducedDebug

Whether the "reducedDebugInfo" option is active for this player.

Returns boolean

```zenscript
myMCPlayerEntity.hasReducedDebug();
```

### hashCode

Returns int

```zenscript
myMCPlayerEntity.hashCode();
```

### heal

Heal living entity (param: amount of half-hearts)

```zenscript
myMCPlayerEntity.heal(healAmount as float);
```

| Parameter  | Type  | Description             |
| ---------- | ----- | ----------------------- |
| healAmount | float | No description provided |


### ignoreItemEntityData

Checks if players can use this entity to access operator (permission level 2) commands either directly or indirectly, such as give or setblock. A similar method exists for entities at {@link net.minecraft.tileentity.TileEntity#onlyOpsCanSetNbt()}.<p>For example, {@link
 net.minecraft.entity.item.EntityMinecartCommandBlock#ignoreItemEntityData() command block minecarts} and {@link
 net.minecraft.entity.item.EntityMinecartMobSpawner#ignoreItemEntityData() mob spawner minecarts} (spawning command
 block minecarts or drops) are considered accessible.</p>Returns: `true if this entity offers ways for unauthorized
 players to use restricted commands`

Returns boolean

```zenscript
myMCPlayerEntity.ignoreItemEntityData();
```

### isActiveItemStackBlocking

Returns boolean

```zenscript
myMCPlayerEntity.isActiveItemStackBlocking();
```

### isAddedToWorld

Returns boolean

```zenscript
myMCPlayerEntity.isAddedToWorld();
```

### isAlive

Returns true if the entity has not been .

Returns boolean

```zenscript
myMCPlayerEntity.isAlive();
```

### isAllowEdit

Returns boolean

```zenscript
myMCPlayerEntity.isAllowEdit();
```

### isBeingRidden

If at least 1 entity is riding this one

Returns boolean

```zenscript
myMCPlayerEntity.isBeingRidden();
```

### isBurning

Returns true if the entity is on fire. Used by render to add the fire effect on rendering.

Returns boolean

```zenscript
myMCPlayerEntity.isBurning();
```

### isChild

If Animal, checks if the age timer is negative

Returns boolean

```zenscript
myMCPlayerEntity.isChild();
```

### isCreative

Returns boolean

```zenscript
myMCPlayerEntity.isCreative();
```

### isCustomNameVisible

Returns boolean

```zenscript
myMCPlayerEntity.isCustomNameVisible();
```

### isElytraFlying

Returns boolean

```zenscript
myMCPlayerEntity.isElytraFlying();
```

### isEntityInsideOpaqueBlock

Checks if this entity is inside of an opaque block

Returns boolean

```zenscript
myMCPlayerEntity.isEntityInsideOpaqueBlock();
```

### isEntityUndead

Returns true if this entity is undead.

Returns boolean

```zenscript
myMCPlayerEntity.isEntityUndead();
```

### isGlowing

Returns boolean

```zenscript
myMCPlayerEntity.isGlowing();
```

### isHandActive

Returns boolean

```zenscript
myMCPlayerEntity.isHandActive();
```

### isImmuneToExplosions

Returns boolean

```zenscript
myMCPlayerEntity.isImmuneToExplosions();
```

### isImmuneToFire

Returns boolean

```zenscript
myMCPlayerEntity.isImmuneToFire();
```

### isInLava

Returns boolean

```zenscript
myMCPlayerEntity.isInLava();
```

### isInRangeToRender3d

Returns boolean

```zenscript
myMCPlayerEntity.isInRangeToRender3d(x as double, y as double, z as double);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| x         | double | No description provided |
| y         | double | No description provided |
| z         | double | No description provided |


### isInRangeToRenderDist

Checks if the entity is in range to render.

Returns boolean

```zenscript
myMCPlayerEntity.isInRangeToRenderDist(distance as double);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| distance  | double | No description provided |


### isInWater

Checks if this entity is inside water (if inWater field is true as a result of handleWaterMovement() returning true)

Returns boolean

```zenscript
myMCPlayerEntity.isInWater();
```

### isInWaterOrBubbleColumn

Returns boolean

```zenscript
myMCPlayerEntity.isInWaterOrBubbleColumn();
```

### isInWaterRainOrBubbleColumn

Returns boolean

```zenscript
myMCPlayerEntity.isInWaterRainOrBubbleColumn();
```

### isInvisible

Returns boolean

```zenscript
myMCPlayerEntity.isInvisible();
```

### isInvisibleToPlayer

Only used by renderer in EntityLivingBase subclasses. Determines if an entity is visible or not to a specific player, if the entity is normally invisible. For EntityLivingBase subclasses, returning false when invisible will render the entity semi-transparent.

Returns boolean

```zenscript
myMCPlayerEntity.isInvisibleToPlayer(player as crafttweaker.api.entity.player.MCPlayerEntity);
```

| Parameter | Type                                                                                       | Description             |
| --------- | ------------------------------------------------------------------------------------------ | ----------------------- |
| player    | [crafttweaker.api.entity.player.MCPlayerEntity](/vanilla/api/entity/player/MCPlayerEntity) | No description provided |


### isInvulnerable

Returns boolean

```zenscript
myMCPlayerEntity.isInvulnerable();
```

### isLiving

Returns boolean

```zenscript
myMCPlayerEntity.isLiving();
```

### isNonBoss

Returns false if this Entity is a boss, true otherwise.

Returns boolean

```zenscript
myMCPlayerEntity.isNonBoss();
```

### isOffsetPositionInLiquid

Checks if the offset position from the entity's current position is inside of a liquid.

Returns boolean

```zenscript
myMCPlayerEntity.isOffsetPositionInLiquid(x as double, y as double, z as double);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| x         | double | No description provided |
| y         | double | No description provided |
| z         | double | No description provided |


### isOnLadder

Returns true if this entity should move as if it were on a ladder (either because it's actually on a ladder, or for AI reasons)

Returns boolean

```zenscript
myMCPlayerEntity.isOnLadder();
```

### isOnePlayerRiding

Returns boolean

```zenscript
myMCPlayerEntity.isOnePlayerRiding();
```

### isPassenger

Returns boolean

```zenscript
myMCPlayerEntity.isPassenger();
```

### isPlayerFullyAsleep

Returns whether or not the player is asleep and the screen has fully faded.

Returns boolean

```zenscript
myMCPlayerEntity.isPlayerFullyAsleep();
```

### isPotionActive

Returns boolean

```zenscript
myMCPlayerEntity.isPotionActive(potionIn as crafttweaker.api.potion.MCPotionEffect);
```

| Parameter | Type                                                                          | Description             |
| --------- | ----------------------------------------------------------------------------- | ----------------------- |
| potionIn  | [crafttweaker.api.potion.MCPotionEffect](/vanilla/api/potions/MCPotionEffect) | No description provided |


### isPotionApplicable

Returns boolean

```zenscript
myMCPlayerEntity.isPotionApplicable(potioneffectIn as crafttweaker.api.potion.MCPotionEffectInstance);
```

| Parameter      | Type                                                                                          | Description             |
| -------------- | --------------------------------------------------------------------------------------------- | ----------------------- |
| potioneffectIn | [crafttweaker.api.potion.MCPotionEffectInstance](/vanilla/api/potions/MCPotionEffectInstance) | No description provided |


### isPushedByWater

Returns boolean

```zenscript
myMCPlayerEntity.isPushedByWater();
```

### isServerWorld

Returns whether the entity is in a server world

Returns boolean

```zenscript
myMCPlayerEntity.isServerWorld();
```

### isSilent

Returns: `True if this entity will not play sounds`

Returns boolean

```zenscript
myMCPlayerEntity.isSilent();
```

### isSleeping

Returns whether player is sleeping or not

Returns boolean

```zenscript
myMCPlayerEntity.isSleeping();
```

### isSneaking

Returns if this entity is sneaking.

Returns boolean

```zenscript
myMCPlayerEntity.isSneaking();
```

### isSpawnForced

Returns boolean

```zenscript
myMCPlayerEntity.isSpawnForced();
```

### isSpectator

Returns true if the player is in spectator mode.

Returns boolean

```zenscript
myMCPlayerEntity.isSpectator();
```

### isSpinAttacking

Returns boolean

```zenscript
myMCPlayerEntity.isSpinAttacking();
```

### isSprinting

Get if the Entity is sprinting.

Returns boolean

```zenscript
myMCPlayerEntity.isSprinting();
```

### isSwimming

Returns boolean

```zenscript
myMCPlayerEntity.isSwimming();
```

### isUser

returns true if this is an EntityPlayerSP, or the logged in player.

Returns boolean

```zenscript
myMCPlayerEntity.isUser();
```

### isWet

Checks if this entity is either in water or on an open air block in rain (used in wolves).

Returns boolean

```zenscript
myMCPlayerEntity.isWet();
```

### jump

Causes this entity to do an upwards motion (jumping).

```zenscript
myMCPlayerEntity.jump();
```

### livingTick

Called frequently so the entity can update its state every tick as required. For example, zombies and skeletons use this to react to sunlight and start to burn.

```zenscript
myMCPlayerEntity.livingTick();
```

### moveToBlockPosAndAngles

```zenscript
myMCPlayerEntity.moveToBlockPosAndAngles(pos as crafttweaker.api.util.BlockPos, rotationYawIn as float, rotationPitchIn as float);
```

| Parameter       | Type                                                         | Description             |
| --------------- | ------------------------------------------------------------ | ----------------------- |
| pos             | [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos) | No description provided |
| rotationYawIn   | float                                                        | No description provided |
| rotationPitchIn | float                                                        | No description provided |


### onAddedToWorld

```zenscript
myMCPlayerEntity.onAddedToWorld();
```

### onCollideWithPlayer

Called by a player entity when they collide with an entity

```zenscript
myMCPlayerEntity.onCollideWithPlayer(entityIn as crafttweaker.api.entity.player.MCPlayerEntity);
```

| Parameter | Type                                                                                       | Description             |
| --------- | ------------------------------------------------------------------------------------------ | ----------------------- |
| entityIn  | [crafttweaker.api.entity.player.MCPlayerEntity](/vanilla/api/entity/player/MCPlayerEntity) | No description provided |


### onEnchant

```zenscript
myMCPlayerEntity.onEnchant(enchantedItem as crafttweaker.api.item.IItemStack, cost as int);
```

| Parameter     | Type                                                              | Description             |
| ------------- | ----------------------------------------------------------------- | ----------------------- |
| enchantedItem | [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack) | No description provided |
| cost          | int                                                               | No description provided |


### onEnterBubbleColumn

```zenscript
myMCPlayerEntity.onEnterBubbleColumn(downwards as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| downwards | boolean | No description provided |


### onEnterBubbleColumnWithAirAbove

```zenscript
myMCPlayerEntity.onEnterBubbleColumnWithAirAbove(downwards as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| downwards | boolean | No description provided |


### onKillCommand

Called by the /kill command.

```zenscript
myMCPlayerEntity.onKillCommand();
```

### onRemovedFromWorld

```zenscript
myMCPlayerEntity.onRemovedFromWorld();
```

### performHurtAnimation

Setups the entity to do the hurt animation. Only used by packets in multiplayer.

```zenscript
myMCPlayerEntity.performHurtAnimation();
```

### preparePlayerToSpawn

Keeps moving the entity up so it isn't colliding with blocks and other requirements for this entity to be spawned (only actually used on players though its also on Entity)

```zenscript
myMCPlayerEntity.preparePlayerToSpawn();
```

### recalculateSize

```zenscript
myMCPlayerEntity.recalculateSize();
```

### remove

```zenscript
myMCPlayerEntity.remove();
```


```zenscript
myMCPlayerEntity.remove(keepData as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| keepData  | boolean | No description provided |


### removeActivePotionEffect

Returns [crafttweaker.api.potion.MCPotionEffectInstance](/vanilla/api/potions/MCPotionEffectInstance)

```zenscript
myMCPlayerEntity.removeActivePotionEffect(arg0 as crafttweaker.api.potion.MCPotionEffect);
```

| Parameter | Type                                                                          | Description             |
| --------- | ----------------------------------------------------------------------------- | ----------------------- |
| arg0      | [crafttweaker.api.potion.MCPotionEffect](/vanilla/api/potions/MCPotionEffect) | No description provided |


### removePassengers

Dismounts all entities riding this entity from this entity.

```zenscript
myMCPlayerEntity.removePassengers();
```

### removePotionEffect

Returns boolean

```zenscript
myMCPlayerEntity.removePotionEffect(effectIn as crafttweaker.api.potion.MCPotionEffect);
```

| Parameter | Type                                                                          | Description             |
| --------- | ----------------------------------------------------------------------------- | ----------------------- |
| effectIn  | [crafttweaker.api.potion.MCPotionEffect](/vanilla/api/potions/MCPotionEffect) | No description provided |


### removeTag

Returns boolean

```zenscript
myMCPlayerEntity.removeTag(tag as String);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| tag       | String | No description provided |


### replaceItemInInventory

Returns boolean

```zenscript
myMCPlayerEntity.replaceItemInInventory(inventorySlot as int, itemStackIn as crafttweaker.api.item.IItemStack);
```

| Parameter     | Type                                                              | Description             |
| ------------- | ----------------------------------------------------------------- | ----------------------- |
| inventorySlot | int                                                               | No description provided |
| itemStackIn   | [crafttweaker.api.item.IItemStack](/vanilla/api/items/IItemStack) | No description provided |


### resetActiveHand

```zenscript
myMCPlayerEntity.resetActiveHand();
```

### resetCooldown

```zenscript
myMCPlayerEntity.resetCooldown();
```

### resetPositionToBB

Resets the entity's position to the center (planar) and bottom (vertical) points of its bounding box.

```zenscript
myMCPlayerEntity.resetPositionToBB();
```

### respawnPlayer

```zenscript
myMCPlayerEntity.respawnPlayer();
```

### revive

```zenscript
myMCPlayerEntity.revive();
```

### rotateTowards

```zenscript
myMCPlayerEntity.rotateTowards(yaw as double, pitch as double);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| yaw       | double | No description provided |
| pitch     | double | No description provided |


### sendEndCombat

Sends an END_COMBAT packet to the client

```zenscript
myMCPlayerEntity.sendEndCombat();
```

### sendEnterCombat

Sends an ENTER_COMBAT packet to the client

```zenscript
myMCPlayerEntity.sendEnterCombat();
```

### sendPlayerAbilities

Sends the player's abilities to the server (if there is one).

```zenscript
myMCPlayerEntity.sendPlayerAbilities();
```

### setAIMoveSpeed

set the movespeed used for the new AI system

```zenscript
myMCPlayerEntity.setAIMoveSpeed(speedIn as float);
```

| Parameter | Type  | Description             |
| --------- | ----- | ----------------------- |
| speedIn   | float | No description provided |


### setAbsorptionAmount

```zenscript
myMCPlayerEntity.setAbsorptionAmount(amount as float);
```

| Parameter | Type  | Description             |
| --------- | ----- | ----------------------- |
| amount    | float | No description provided |


### setAir

```zenscript
myMCPlayerEntity.setAir(air as int);
```

| Parameter | Type | Description             |
| --------- | ---- | ----------------------- |
| air       | int  | No description provided |


### setArrowCountInEntity

```zenscript
myMCPlayerEntity.setArrowCountInEntity(count as int);
```

| Parameter | Type | Description             |
| --------- | ---- | ----------------------- |
| count     | int  | No description provided |


### setBedPosition

```zenscript
myMCPlayerEntity.setBedPosition(p_213369_1_ as crafttweaker.api.util.BlockPos);
```

| Parameter     | Type                                                         | Description             |
| ------------- | ------------------------------------------------------------ | ----------------------- |
| p_213369_1_ | [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos) | No description provided |


### setCustomNameVisible

```zenscript
myMCPlayerEntity.setCustomNameVisible(alwaysRenderNameTag as boolean);
```

| Parameter           | Type    | Description             |
| ------------------- | ------- | ----------------------- |
| alwaysRenderNameTag | boolean | No description provided |


### setEntityId

```zenscript
myMCPlayerEntity.setEntityId(id as int);
```

| Parameter | Type | Description             |
| --------- | ---- | ----------------------- |
| id        | int  | No description provided |


### setFire

Sets entity to burn for x amount of seconds, cannot lower amount of existing fire.

```zenscript
myMCPlayerEntity.setFire(seconds as int);
```

| Parameter | Type | Description             |
| --------- | ---- | ----------------------- |
| seconds   | int  | No description provided |


### setFireTimer

```zenscript
myMCPlayerEntity.setFireTimer(p_223308_1_ as int);
```

| Parameter     | Type | Description             |
| ------------- | ---- | ----------------------- |
| p_223308_1_ | int  | No description provided |


### setGlowing

```zenscript
myMCPlayerEntity.setGlowing(glowingIn as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| glowingIn | boolean | No description provided |


### setHeadRotation

```zenscript
myMCPlayerEntity.setHeadRotation(yaw as float, pitch as int);
```

| Parameter | Type  | Description             |
| --------- | ----- | ----------------------- |
| yaw       | float | No description provided |
| pitch     | int   | No description provided |


### setHealth

```zenscript
myMCPlayerEntity.setHealth(health as float);
```

| Parameter | Type  | Description             |
| --------- | ----- | ----------------------- |
| health    | float | No description provided |


### setIdleTime

```zenscript
myMCPlayerEntity.setIdleTime(idleTimeIn as int);
```

| Parameter  | Type | Description             |
| ---------- | ---- | ----------------------- |
| idleTimeIn | int  | No description provided |


### setInLava

```zenscript
myMCPlayerEntity.setInLava();
```

### setInvisible

```zenscript
myMCPlayerEntity.setInvisible(invisible as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| invisible | boolean | No description provided |


### setInvulnerable

Sets whether this Entity is invulnerable.

```zenscript
myMCPlayerEntity.setInvulnerable(isInvulnerable as boolean);
```

| Parameter      | Type    | Description             |
| -------------- | ------- | ----------------------- |
| isInvulnerable | boolean | No description provided |


### setJumping

```zenscript
myMCPlayerEntity.setJumping(jumping as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| jumping   | boolean | No description provided |


### setLocationAndAngles

Sets the location and Yaw/Pitch of an entity in the world

```zenscript
myMCPlayerEntity.setLocationAndAngles(x as double, y as double, z as double, yaw as float, pitch as float);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| x         | double | No description provided |
| y         | double | No description provided |
| z         | double | No description provided |
| yaw       | float  | No description provided |
| pitch     | float  | No description provided |


### setMotion

```zenscript
myMCPlayerEntity.setMotion(x as double, y as double, z as double);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| x         | double | No description provided |
| y         | double | No description provided |
| z         | double | No description provided |


### setNoGravity

```zenscript
myMCPlayerEntity.setNoGravity(noGravity as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| noGravity | boolean | No description provided |


### setPartying

Called when a record starts or stops playing. Used to make parrots start or stop partying.

```zenscript
myMCPlayerEntity.setPartying(pos as crafttweaker.api.util.BlockPos, isPartying as boolean);
```

| Parameter  | Type                                                         | Description             |
| ---------- | ------------------------------------------------------------ | ----------------------- |
| pos        | [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos) | No description provided |
| isPartying | boolean                                                      | No description provided |


### setPortal

Marks the entity as being inside a portal, activating teleportation logic in onEntityUpdate() in the following tick(s).

```zenscript
myMCPlayerEntity.setPortal(pos as crafttweaker.api.util.BlockPos);
```

| Parameter | Type                                                         | Description             |
| --------- | ------------------------------------------------------------ | ----------------------- |
| pos       | [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos) | No description provided |


### setPosition

Sets the x,y,z of the entity from the given parameters. Also seems to set up a bounding box.

```zenscript
myMCPlayerEntity.setPosition(x as double, y as double, z as double);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| x         | double | No description provided |
| y         | double | No description provided |
| z         | double | No description provided |


### setPositionAndRotation

Sets position and rotation, clamping and wrapping params to valid values. Used by network code.

```zenscript
myMCPlayerEntity.setPositionAndRotation(x as double, y as double, z as double, yaw as float, pitch as float);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| x         | double | No description provided |
| y         | double | No description provided |
| z         | double | No description provided |
| yaw       | float  | No description provided |
| pitch     | float  | No description provided |


### setPositionAndRotationDirect

Sets a target for the client to interpolate towards over the next few ticks

```zenscript
myMCPlayerEntity.setPositionAndRotationDirect(x as double, y as double, z as double, yaw as float, pitch as float, posRotationIncrements as int, teleport as boolean);
```

| Parameter             | Type    | Description             |
| --------------------- | ------- | ----------------------- |
| x                     | double  | No description provided |
| y                     | double  | No description provided |
| z                     | double  | No description provided |
| yaw                   | float   | No description provided |
| pitch                 | float   | No description provided |
| posRotationIncrements | int     | No description provided |
| teleport              | boolean | No description provided |


### setPositionAndUpdate

Sets the position of the entity and updates the 'last' variables

```zenscript
myMCPlayerEntity.setPositionAndUpdate(x as double, y as double, z as double);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| x         | double | No description provided |
| y         | double | No description provided |
| z         | double | No description provided |


### setPositionNonDirty

Returns boolean

```zenscript
myMCPlayerEntity.setPositionNonDirty();
```

### setReducedDebug

```zenscript
myMCPlayerEntity.setReducedDebug(reducedDebug as boolean);
```

| Parameter    | Type    | Description             |
| ------------ | ------- | ----------------------- |
| reducedDebug | boolean | No description provided |


### setRenderYawOffset

Set the render yaw offset

```zenscript
myMCPlayerEntity.setRenderYawOffset(offset as float);
```

| Parameter | Type  | Description             |
| --------- | ----- | ----------------------- |
| offset    | float | No description provided |


### setRotationYawHead

Sets the head's yaw rotation of the entity.

```zenscript
myMCPlayerEntity.setRotationYawHead(rotation as float);
```

| Parameter | Type  | Description             |
| --------- | ----- | ----------------------- |
| rotation  | float | No description provided |


### setScore

Set player's score

```zenscript
myMCPlayerEntity.setScore(scoreIn as int);
```

| Parameter | Type | Description             |
| --------- | ---- | ----------------------- |
| scoreIn   | int  | No description provided |


### setSilent

When set to true the entity will not play sounds.

```zenscript
myMCPlayerEntity.setSilent(isSilent as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| isSilent  | boolean | No description provided |


### setSneaking

Sets the sneaking flag.

```zenscript
myMCPlayerEntity.setSneaking(sneaking as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| sneaking  | boolean | No description provided |


### setSpawnPoint

```zenscript
myMCPlayerEntity.setSpawnPoint(pos as crafttweaker.api.util.BlockPos, forced as boolean);
```

| Parameter | Type                                                         | Description             |
| --------- | ------------------------------------------------------------ | ----------------------- |
| pos       | [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos) | No description provided |
| forced    | boolean                                                      | No description provided |


### setSprinting

Set sprinting switch for Entity.

```zenscript
myMCPlayerEntity.setSprinting(sprinting as boolean);
```

| Parameter | Type    | Description             |
| --------- | ------- | ----------------------- |
| sprinting | boolean | No description provided |


### setSwimming

```zenscript
myMCPlayerEntity.setSwimming(p_204711_1_ as boolean);
```

| Parameter     | Type    | Description             |
| ------------- | ------- | ----------------------- |
| p_204711_1_ | boolean | No description provided |


### setVelocity

Updates the entity motion clientside, called by packets from the server

```zenscript
myMCPlayerEntity.setVelocity(x as double, y as double, z as double);
```

| Parameter | Type   | Description             |
| --------- | ------ | ----------------------- |
| x         | double | No description provided |
| y         | double | No description provided |
| z         | double | No description provided |


### shouldHeal

Checks if the player's health is not full and not zero.

Returns boolean

```zenscript
myMCPlayerEntity.shouldHeal();
```

### shouldReceiveErrors

Returns boolean

```zenscript
myMCPlayerEntity.shouldReceiveErrors();
```

### shouldReceiveFeedback

Returns boolean

```zenscript
myMCPlayerEntity.shouldReceiveFeedback();
```

### shouldRenderSneaking

Returns boolean

```zenscript
myMCPlayerEntity.shouldRenderSneaking();
```

### shouldRiderFaceForward

Returns true if the entity's rider (EntityPlayer) should face forward when mounted. currently only used in vanilla code by pigs.

Returns boolean

```zenscript
myMCPlayerEntity.shouldRiderFaceForward(player as crafttweaker.api.entity.player.MCPlayerEntity);
```

| Parameter | Type                                                                                       | Description                          |
| --------- | ------------------------------------------------------------------------------------------ | ------------------------------------ |
| player    | [crafttweaker.api.entity.player.MCPlayerEntity](/vanilla/api/entity/player/MCPlayerEntity) | The player who is riding the entity. |


### shouldRiderSit

Returns boolean

```zenscript
myMCPlayerEntity.shouldRiderSit();
```

### spawnRunningParticles

Attempts to create sprinting particles if the entity is sprinting and not in water.

```zenscript
myMCPlayerEntity.spawnRunningParticles();
```

### spawnSweepParticles

```zenscript
myMCPlayerEntity.spawnSweepParticles();
```

### startSleeping

```zenscript
myMCPlayerEntity.startSleeping(p_213342_1_ as crafttweaker.api.util.BlockPos);
```

| Parameter     | Type                                                         | Description             |
| ------------- | ------------------------------------------------------------ | ----------------------- |
| p_213342_1_ | [crafttweaker.api.util.BlockPos](/vanilla/api/util/BlockPos) | No description provided |


### startSpinAttack

```zenscript
myMCPlayerEntity.startSpinAttack(p_204803_1_ as int);
```

| Parameter     | Type | Description             |
| ------------- | ---- | ----------------------- |
| p_204803_1_ | int  | No description provided |


### stopActiveHand

```zenscript
myMCPlayerEntity.stopActiveHand();
```

### stopRiding

Dismounts this entity from the entity it is riding.

```zenscript
myMCPlayerEntity.stopRiding();
```

### teleportKeepLoaded

```zenscript
myMCPlayerEntity.teleportKeepLoaded(p_223102_1_ as double, p_223102_3_ as double, p_223102_5_ as double);
```

| Parameter     | Type   | Description             |
| ------------- | ------ | ----------------------- |
| p_223102_1_ | double | No description provided |
| p_223102_3_ | double | No description provided |
| p_223102_5_ | double | No description provided |


### tick

Called to update the entity's position/logic.

```zenscript
myMCPlayerEntity.tick();
```

### toString

Returns String

```zenscript
myMCPlayerEntity.toString();
```

### updateRidden

Handles updating while riding another entity

```zenscript
myMCPlayerEntity.updateRidden();
```

### updateSwimming

```zenscript
myMCPlayerEntity.updateSwimming();
```

### wakeUp

```zenscript
myMCPlayerEntity.wakeUp();
```

### wakeUpPlayer

Wake up the player if they're sleeping.

```zenscript
myMCPlayerEntity.wakeUpPlayer(immediately as boolean, updateWorldFlag as boolean, setSpawn as boolean);
```

| Parameter       | Type    | Description             |
| --------------- | ------- | ----------------------- |
| immediately     | boolean | No description provided |
| updateWorldFlag | boolean | No description provided |
| setSpawn        | boolean | No description provided |


### xpBarCap

This method returns the cap amount of experience that the experience bar can hold. With each level, the experience cap on the player's experience bar is raised by 10.

Returns int

```zenscript
myMCPlayerEntity.xpBarCap();
```

