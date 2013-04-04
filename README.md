NEIcrashlog
===========

Here is the crash log I'm getting:

---- Minecraft Crash Report ----
// I feel sad now :(

Time: 4/4/13 7:56 AM
Description: Updating screen events

java.lang.ClassCastException: java.util.ArrayList cannot be cast to net.minecraft.item.ItemStack
  at factorization.common.TileEntityMixer$RecipeMatchInfo.<init>(TileEntityMixer.java:229)
	at factorization.common.TileEntityMixer.getRecipes(TileEntityMixer.java:334)
	at factorization.nei.NEI_MixerRecipeConfig.getCache(NEI_MixerRecipeConfig.java:57)
	at factorization.nei.NEI_MixerRecipeConfig.loadCraftingRecipes(NEI_MixerRecipeConfig.java:41)
	at codechicken.nei.recipe.TemplateRecipeHandler.loadCraftingRecipes(TemplateRecipeHandler.java:351)
	at factorization.nei.NEI_MixerRecipeConfig.loadCraftingRecipes(NEI_MixerRecipeConfig.java:68)
	at codechicken.nei.recipe.TemplateRecipeHandler.getRecipeHandler(TemplateRecipeHandler.java:497)
	at codechicken.nei.recipe.GuiCraftingRecipe.openRecipeGui(GuiCraftingRecipe.java:39)
	at codechicken.nei.recipe.RecipeItemInputHandler.lastKeyTyped(RecipeItemInputHandler.java:22)
	at codechicken.nei.forge.GuiContainerManager.lastKeyTyped(GuiContainerManager.java:434)
	at net.minecraft.client.gui.inventory.GuiContainer.func_73869_a(GuiContainer.java:862)
	at net.minecraft.client.gui.inventory.GuiContainer.func_73860_n(GuiContainer.java:954)
	at net.minecraft.client.gui.GuiScreen.func_73862_m(SourceFile:115)
	at net.minecraft.client.Minecraft.func_71407_l(Minecraft.java:1496)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:831)
	at net.minecraft.client.Minecraft.run(Minecraft.java:756)
	at java.lang.Thread.run(Unknown Source)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at factorization.common.TileEntityMixer$RecipeMatchInfo.<init>(TileEntityMixer.java:229)
	at factorization.common.TileEntityMixer.getRecipes(TileEntityMixer.java:334)
	at factorization.nei.NEI_MixerRecipeConfig.getCache(NEI_MixerRecipeConfig.java:57)
	at factorization.nei.NEI_MixerRecipeConfig.loadCraftingRecipes(NEI_MixerRecipeConfig.java:41)
	at codechicken.nei.recipe.TemplateRecipeHandler.loadCraftingRecipes(TemplateRecipeHandler.java:351)
	at factorization.nei.NEI_MixerRecipeConfig.loadCraftingRecipes(NEI_MixerRecipeConfig.java:68)
	at codechicken.nei.recipe.TemplateRecipeHandler.getRecipeHandler(TemplateRecipeHandler.java:497)
	at codechicken.nei.recipe.GuiCraftingRecipe.openRecipeGui(GuiCraftingRecipe.java:39)
	at codechicken.nei.recipe.RecipeItemInputHandler.lastKeyTyped(RecipeItemInputHandler.java:22)
	at codechicken.nei.forge.GuiContainerManager.lastKeyTyped(GuiContainerManager.java:434)
	at net.minecraft.client.gui.inventory.GuiContainer.func_73869_a(GuiContainer.java:862)
	at net.minecraft.client.gui.inventory.GuiContainer.func_73860_n(GuiContainer.java:954)
	at net.minecraft.client.gui.GuiScreen.func_73862_m(SourceFile:115)

-- Affected screen --
Details:
	Screen name: codechicken.nei.GuiExtendedCreativeInv

-- Affected level --
Details:
	Level name: MpServer
	All players: 1 total; [EntityClientPlayerMP['Oodahn'/264, l='MpServer', x=-578.67, y=70.62, z=1226.16]]
	Chunk stats: MultiplayerChunkCache: 441
	Level seed: 0
	Level generator: ID 04 - BIOMESOP, ver 0. Features enabled: false
	Level generator options: 
	Level spawn location: World: (184,64,256), Chunk: (at 8,4,0 in 11,16; contains blocks 176,0,256 to 191,255,271), Region: (0,0; contains chunks 0,0 to 31,31, blocks 0,0,0 to 511,255,511)
	Level time: 135529 game time, 206381 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: false), thunder time: 0 (now: false)
	Level game mode: Game mode: creative (ID 1). Hardcore: false. Cheats: false
	Forced entities: 111 total; [EntityBat['Bat'/1641, l='MpServer', x=-500.42, y=20.02, z=1279.42], EntityClientPlayerMP['Oodahn'/264, l='MpServer', x=-578.67, y=70.62, z=1226.16], EntityCreeper['Creeper'/553, l='MpServer', x=-531.50, y=22.00, z=1289.50], EntityVillager['Villager'/258, l='MpServer', x=-516.78, y=66.00, z=1201.47], EntityVillager['Villager'/259, l='MpServer', x=-517.31, y=66.00, z=1200.59], EntityVillager['Villager'/256, l='MpServer', x=-523.56, y=66.00, z=1213.75], EntityVillager['Villager'/257, l='MpServer', x=-518.56, y=66.00, z=1201.70], EntityPig['Pig'/262, l='MpServer', x=-522.50, y=66.00, z=1194.66], EntityPig['Pig'/263, l='MpServer', x=-522.22, y=67.00, z=1190.53], EntityVillager['Villager'/260, l='MpServer', x=-519.37, y=66.00, z=1201.18], EntityVillager['Villager'/261, l='MpServer', x=-517.85, y=66.00, z=1201.69], EntityItem['item.tile.log.oak'/265, l='MpServer', x=-587.38, y=70.13, z=1228.13], EntitySkeleton['Skeleton'/572, l='MpServer', x=-591.66, y=64.00, z=1285.88], EntityBat['Bat'/1652, l='MpServer', x=-620.67, y=35.88, z=1256.48], EntityPig['Pig'/343, l='MpServer', x=-652.31, y=66.00, z=1208.50], EntityPig['Pig'/342, l='MpServer', x=-644.84, y=63.00, z=1203.47], EntityPig['Pig'/341, l='MpServer', x=-647.25, y=63.00, z=1213.88], EntityPig['Pig'/340, l='MpServer', x=-639.09, y=63.00, z=1214.25], EntityPig['Pig'/339, l='MpServer', x=-656.97, y=63.00, z=1214.13], EntityPig['Pig'/338, l='MpServer', x=-643.50, y=64.00, z=1198.50], EntityMinecartChest['entity.MinecartChest.name'/337, l='MpServer', x=-650.50, y=37.50, z=1163.50], EntityPig['Pig'/348, l='MpServer', x=-641.50, y=64.00, z=1301.50], EntityPig['Pig'/347, l='MpServer', x=-642.47, y=63.00, z=1303.50], EntityPig['Pig'/346, l='MpServer', x=-644.50, y=64.00, z=1292.31], EntityCreeper['Creeper'/345, l='MpServer', x=-649.50, y=36.00, z=1280.50], EntityPig['Pig'/344, l='MpServer', x=-642.25, y=64.00, z=1204.09], EntityCreeper['Creeper'/373, l='MpServer', x=-615.97, y=21.00, z=1305.47], EntitySquid['Squid'/372, l='MpServer', x=-613.47, y=58.00, z=1207.69], EntitySquid['Squid'/369, l='MpServer', x=-616.50, y=60.34, z=1208.88], EntityCreeper['Creeper'/368, l='MpServer', x=-613.13, y=64.00, z=1159.25], EntitySquid['Squid'/371, l='MpServer', x=-612.81, y=60.19, z=1208.56], EntitySquid['Squid'/370, l='MpServer', x=-616.50, y=58.00, z=1213.50], EntitySquid['Squid'/383, l='MpServer', x=-598.88, y=60.00, z=1196.88], EntitySquid['Squid'/382, l='MpServer', x=-595.50, y=59.00, z=1195.72], EntityCreeper['Creeper'/357, l='MpServer', x=-627.50, y=44.00, z=1166.50], EntityCreeper['Creeper'/358, l='MpServer', x=-626.50, y=44.00, z=1173.50], EntityCreeper['Creeper'/359, l='MpServer', x=-625.50, y=44.00, z=1174.50], EntitySkeleton['Skeleton'/364, l='MpServer', x=-628.31, y=29.00, z=1304.78], EntityZombie['Zombie'/601, l='MpServer', x=-531.50, y=64.00, z=1158.50], EntityCreeper['Creeper'/360, l='MpServer', x=-628.50, y=44.00, z=1169.50], EntityMinecartChest['entity.MinecartChest.name'/361, l='MpServer', x=-637.50, y=33.50, z=1187.50], EntityZombie['Zombie'/604, l='MpServer', x=-531.50, y=64.00, z=1152.50], EntityPig['Pig'/362, l='MpServer', x=-638.97, y=63.00, z=1215.97], EntityCreeper['Creeper'/363, l='MpServer', x=-638.69, y=63.00, z=1229.47], EntityEnderman['Enderman'/410, l='MpServer', x=-547.91, y=40.00, z=1266.66], EntityBat['Bat'/411, l='MpServer', x=-551.41, y=39.10, z=1307.47], EntityCreeper['Creeper'/408, l='MpServer', x=-558.50, y=43.00, z=1275.50], EntityCreeper['Creeper'/409, l='MpServer', x=-558.50, y=43.00, z=1277.50], EntityPig['Pig'/402, l='MpServer', x=-549.50, y=67.00, z=1218.50], EntityZombie['Zombie'/403, l='MpServer', x=-538.91, y=21.00, z=1233.47], EntityPig['Pig'/401, l='MpServer', x=-548.50, y=66.00, z=1210.69], EntityEnderman['Enderman'/406, l='MpServer', x=-551.31, y=36.47, z=1266.50], EntitySpider['Spider'/407, l='MpServer', x=-550.94, y=66.00, z=1261.03], EntityCreeper['Creeper'/404, l='MpServer', x=-548.34, y=18.00, z=1246.09], EntityEnderman['Enderman'/405, l='MpServer', x=-549.56, y=38.00, z=1264.34], EntityBat['Bat'/395, l='MpServer', x=-571.98, y=42.13, z=1238.56], EntitySkeleton['Skeleton'/394, l='MpServer', x=-570.50, y=18.00, z=1204.50], EntityCreeper['Creeper'/397, l='MpServer', x=-567.34, y=12.00, z=1290.03], EntityBat['Bat'/396, l='MpServer', x=-567.25, y=31.10, z=1248.25], EntityZombie['Zombie'/387, l='MpServer', x=-596.50, y=38.00, z=1289.50], EntityZombie['Zombie'/386, l='MpServer', x=-589.50, y=39.00, z=1291.94], EntitySquid['Squid'/385, l='MpServer', x=-602.50, y=60.28, z=1201.78], EntitySquid['Squid'/384, l='MpServer', x=-601.72, y=60.16, z=1199.50], EntityZombie['Zombie'/391, l='MpServer', x=-581.50, y=65.00, z=1170.94], EntityZombie['Zombie'/390, l='MpServer', x=-583.50, y=66.00, z=1176.50], EntitySkeleton['Skeleton'/388, l='MpServer', x=-598.50, y=38.00, z=1294.50], EntityBat['Bat'/440, l='MpServer', x=-542.75, y=39.21, z=1268.93], EntitySkeleton['Skeleton'/441, l='MpServer', x=-534.50, y=17.00, z=1269.50], EntitySkeleton['Skeleton'/442, l='MpServer', x=-531.09, y=17.00, z=1270.31], EntityCreeper['Creeper'/443, l='MpServer', x=-546.41, y=18.00, z=1269.00], EntityPig['Pig'/432, l='MpServer', x=-535.91, y=71.00, z=1204.13], EntityPig['Pig'/433, l='MpServer', x=-537.16, y=67.00, z=1220.06], EntitySkeleton['Skeleton'/434, l='MpServer', x=-537.56, y=67.00, z=1227.09], EntitySkeleton['Skeleton'/435, l='MpServer', x=-531.69, y=20.00, z=1247.44], EntityBat['Bat'/436, l='MpServer', x=-529.50, y=21.10, z=1240.44], EntitySkeleton['Skeleton'/437, l='MpServer', x=-536.50, y=58.00, z=1246.50], EntitySkeleton['Skeleton'/438, l='MpServer', x=-531.50, y=24.00, z=1253.50], EntitySkeleton['Skeleton'/439, l='MpServer', x=-531.69, y=20.00, z=1248.25], EntityPig['Pig'/425, l='MpServer', x=-530.47, y=64.00, z=1171.47], EntityPig['Pig'/424, l='MpServer', x=-531.53, y=64.00, z=1172.53], EntityPig['Pig'/427, l='MpServer', x=-532.50, y=65.00, z=1196.50], EntityPig['Pig'/426, l='MpServer', x=-533.69, y=65.00, z=1180.09], EntityPig['Pig'/429, l='MpServer', x=-529.38, y=66.00, z=1190.19], EntityPig['Pig'/428, l='MpServer', x=-530.75, y=68.00, z=1184.50], EntityPig['Pig'/431, l='MpServer', x=-539.53, y=65.00, z=1211.66], EntityPig['Pig'/430, l='MpServer', x=-532.06, y=66.00, z=1199.06], EntityPig['Pig'/423, l='MpServer', x=-538.78, y=64.00, z=1170.63], EntityZombie['Zombie'/472, l='MpServer', x=-508.59, y=27.00, z=1304.31], EntityCreeper['Creeper'/470, l='MpServer', x=-500.94, y=27.00, z=1306.38], EntityCreeper['Creeper'/471, l='MpServer', x=-506.50, y=27.00, z=1305.84], EntityCreeper['Creeper'/468, l='MpServer', x=-508.50, y=46.00, z=1243.50], EntityBat['Bat'/469, l='MpServer', x=-498.83, y=55.39, z=1279.35], EntityCreeper['Creeper'/466, l='MpServer', x=-502.53, y=65.00, z=1207.31], EntityZombie['Zombie'/467, l='MpServer', x=-511.50, y=34.00, z=1235.50], EntityPig['Pig'/464, l='MpServer', x=-509.53, y=67.00, z=1161.31], EntityPig['Pig'/465, l='MpServer', x=-509.34, y=66.00, z=1182.97], EntityZombie['Zombie'/462, l='MpServer', x=-510.50, y=67.00, z=1147.50], EntityCreeper['Creeper'/458, l='MpServer', x=-527.50, y=58.00, z=1305.50], EntityBat['Bat'/457, l='MpServer', x=-516.77, y=25.00, z=1278.26], EntityBat['Bat'/456, l='MpServer', x=-514.52, y=25.00, z=1273.35], EntityBat['Bat'/455, l='MpServer', x=-513.70, y=54.30, z=1260.75], EntityCreeper['Creeper'/454, l='MpServer', x=-518.03, y=49.00, z=1248.44], EntityZombie['Zombie'/453, l='MpServer', x=-512.50, y=46.00, z=1246.50], EntitySkeleton['Skeleton'/452, l='MpServer', x=-514.50, y=34.00, z=1239.50], EntityPig['Pig'/451, l='MpServer', x=-522.66, y=67.00, z=1172.53], EntityCreeper['Creeper'/450, l='MpServer', x=-518.03, y=17.00, z=1169.38], EntitySpider['Spider'/449, l='MpServer', x=-518.63, y=66.00, z=1151.03], EntitySpider['Spider'/448, l='MpServer', x=-515.00, y=66.00, z=1160.66], EntityVillager['Villager'/254, l='MpServer', x=-524.09, y=65.00, z=1211.60], EntityVillager['Villager'/255, l='MpServer', x=-523.31, y=65.00, z=1208.63], EntityMageVillager['Mage Villager'/253, l='MpServer', x=-514.31, y=66.00, z=1201.69]]
	Retry entities: 0 total; []
Stacktrace:
	at net.minecraft.client.multiplayer.WorldClient.func_72914_a(WorldClient.java:441)
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2405)
	at net.minecraft.client.Minecraft.run(Minecraft.java:772)
	at java.lang.Thread.run(Unknown Source)

-- System Details --
Details:
	Minecraft Version: 1.5.1
	Operating System: Windows 7 (amd64) version 6.1
	Java Version: 1.7.0_11, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 249651536 bytes (238 MB) / 689360896 bytes (657 MB) up to 4260102144 bytes (4062 MB)
	JVM Flags: 8 total; -Xms256M -Xmx4096M -XX:+UseConcMarkSweepGC -XX:+CMSIncrementalMode -XX:+AggressiveOpts -Xms512m -XX:PermSize=128M -XX:MaxPermSize=512m
	AABB Pool Size: 6116 (342496 bytes; 0 MB) allocated, 2 (112 bytes; 0 MB) used
	Suspicious classes: FML and Forge are installed
	IntCache: cache: 0, tcache: 0, allocated: 3, tallocated: 63
	FML: MCP v7.44 FML v5.1.13.629 Minecraft Forge 7.7.1.629 Optifine OptiFine_1.5.1_HD_U_B1 Feed The Beast Mod Pack 30 mods loaded, 30 mods active
	mcp [Minecraft Coder Pack] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	FML [Forge Mod Loader] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Forge [Minecraft Forge] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	CodeChickenCore [CodeChicken Core] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	NotEnoughItems [Not Enough Items] (coremods) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	mod_bspkrsCore [bspkrsCore] ([1.5.1]bspkrsCorev1.03.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	mod_ThebombzenAPI [mod_ThebombzenAPI] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	AutoSwitch [AutoSwitch] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ASVanillaModule [AutoSwitch Vanilla Module] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	TreeCapitator [TreeCapitator] ([1.5.1]TreeCapitator.Forge.1.5.1.r01.Uni.CoreMod.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	mod_ReiMinimap [mod_ReiMinimap] ([1.5.1]ReiMinimap_v3.3_04.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ArsMagica [Ars Magica] (ArsMagica_5.45.011.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Backpack [Backpack] (backpack-1.7.8-1.5.1 (2).zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BetterAnvil [Better Anvils] (betterAnvil - 151 - 4.0.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BiblioCraft [BiblioCraft] (BiblioCraft[v1.1.5].zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BiomesOPlenty [Biomes O' Plenty] (biomes-o-plenty-0.4.8.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Chisel [Chisel] (chisel-1.5.1-1.0.1.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	eplus [Enchanting Plus] (EnchantingPlus-1.5.1-1.14.3.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	EnderStorage [EnderStorage] (EnderStorage 1.4.2.3.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	factorization [Factorization] (Factorization-0.7.23.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	factorization.misc [Factorization Miscellaneous Nonsense] (Factorization-0.7.23.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	factorization.dimensionalSlice [Factorization Dimensional Slices] (Factorization-0.7.23.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Forestry [Forestry for Minecraft] (forestry-A-2.1.0.31.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	inventorytweaks [Inventory Tweaks] (InventoryTweaks-1.52.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	IronChest [Iron Chest] (ironchest-universal-1.5.1-5.2.2.325.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Mystcraft [Mystcraft] (mystcraft-uni-1.5.1-0.10.2.00.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	mod_SmartMoving [Smart Moving] (Smart Moving Universal for ModLoader or Minecraft Forge or MCPC+.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	mod_SmartRender [Smart Render] (Smart Moving Universal for ModLoader or Minecraft Forge or MCPC+.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	StevesCarts [Steve's Carts] (StevesCarts2.0.0.a94.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	TwilightForest [The Twilight Forest] (twilightforest-1.17.1.zip) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	LWJGL: 2.4.2
	OpenGL: GeForce GTS 450/PCIe/SSE2 GL version 4.3.0, NVIDIA Corporation
	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Texture Pack: Default
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 1923 (107688 bytes; 0 MB) allocated, 14 (784 bytes; 0 MB) used
