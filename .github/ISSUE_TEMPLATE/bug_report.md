---
name: Error: java.lang.NullPointerException: Unexpected error
Exit Code: -1
about: Help OptiFine pinpoint issues
title: "optifine 1.16.4 crashes with forge when I open up a world"
labels: ''
assignees: ''

---

## Description of Issue
I want to play MC with forge but I need optifine for my laptop to atleast run the game, but for some reason whenever I try to open a world with both my forge mods and optifine it immedeately crashes

---- Minecraft Crash Report ----
// Surprise! Haha. Well, this is awkward.
 
Time: 12/26/20 1:05 PM
Description: Unexpected error
 
java.lang.NullPointerException: Unexpected error
	at net.minecraft.client.renderer.WorldRenderer.func_228441_a_(WorldRenderer.java:2205) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:structure_gel.mixins.json:WorldRendererMixin,pl:mixin:A}
	at net.minecraft.client.renderer.WorldRenderer.func_228426_a_(WorldRenderer.java:1594) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:structure_gel.mixins.json:WorldRendererMixin,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.func_228378_a_(GameRenderer.java:1022) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.redirect$zje000$redirectRenderingWorld(GameRenderer.java:2110) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.func_195458_a(GameRenderer.java:693) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
	at net.minecraft.client.Minecraft.func_195542_b(Minecraft.java:976) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:imm_ptl_mixins.json:client.MixinMinecraftClient,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinMinecraftClient_B,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:607) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:imm_ptl_mixins.json:client.MixinMinecraftClient,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinMinecraftClient_B,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:184) [?:?] {re:classloading,pl:runtimedistcleaner:A}
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_51] {}
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_51] {}
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_51] {}
	at java.lang.reflect.Method.invoke(Method.java:497) ~[?:1.8.0_51] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider.lambda$launchService$0(FMLClientLaunchProvider.java:51) [forge-1.16.4-35.1.13.jar:35.1] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider$$Lambda$500/1884982716.call(Unknown Source) [forge-1.16.4-35.1.13.jar:35.1] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:37) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:54) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:72) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:82) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:66) [modlauncher-8.0.6.jar:?] {}
 
 
A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------
 
-- Head --
Thread: Render thread
Stacktrace:
	at net.minecraft.client.renderer.WorldRenderer.func_228441_a_(WorldRenderer.java:2205) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:structure_gel.mixins.json:WorldRendererMixin,pl:mixin:A}
	at net.minecraft.client.renderer.WorldRenderer.func_228426_a_(WorldRenderer.java:1594) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:structure_gel.mixins.json:WorldRendererMixin,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.func_228378_a_(GameRenderer.java:1022) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.redirect$zje000$redirectRenderingWorld(GameRenderer.java:2110) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
-- Affected level --
Details:
	All players: 1 total; [ClientPlayerEntity['Oshertree'/376, l='ClientWorld minecraft:overworld', x=119.50, y=4.00, z=-54.50]]
	Chunk stats: Client Chunks (ImmPtl) 529
	Level dimension: minecraft:overworld
	Level spawn location: World: (128,4,-64), Chunk: (at 0,0,0 in 8,-4; contains blocks 128,0,-64 to 143,255,-49), Region: (0,-1; contains chunks 0,-32 to 31,-1, blocks 0,0,-512 to 511,255,-1)
	Level time: 102 game time, 102 day time
	Server brand: forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.world.ClientWorld.func_72914_a(ClientWorld.java:617) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,xf:fml:xaerominimap:xaero_clientworldclass,pl:mixin:APP:mixins.sndctrl.json:MixinClientWorld,pl:mixin:APP:betterweather.mixins.json:client.MixinClientWorld,pl:mixin:A}
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2024) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:imm_ptl_mixins.json:client.MixinMinecraftClient,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinMinecraftClient_B,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:628) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:imm_ptl_mixins.json:client.MixinMinecraftClient,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinMinecraftClient_B,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:184) [?:?] {re:classloading,pl:runtimedistcleaner:A}
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_51] {}
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_51] {}
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_51] {}
	at java.lang.reflect.Method.invoke(Method.java:497) ~[?:1.8.0_51] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider.lambda$launchService$0(FMLClientLaunchProvider.java:51) [forge-1.16.4-35.1.13.jar:35.1] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider$$Lambda$500/1884982716.call(Unknown Source) [forge-1.16.4-35.1.13.jar:35.1] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:37) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:54) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:72) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:82) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:66) [modlauncher-8.0.6.jar:?] {}
 
 
-- System Details --
Details:
	Minecraft Version: 1.16.4
	Minecraft Version ID: 1.16.4
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_51, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 4057567680 bytes (3869 MB) / 6442450944 bytes (6144 MB) up to 6442450944 bytes (6144 MB)
	CPUs: 4
	JVM Flags: 9 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xss1M -Xmx6G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
	ModLauncher: 8.0.6+85+master.325de55
	ModLauncher launch target: fmlclient
	ModLauncher naming: srg
	ModLauncher services: 
		/mixin-0.8.2.jar mixin PLUGINSERVICE 
		/eventbus-3.0.5-service.jar eventbus PLUGINSERVICE 
		/forge-1.16.4-35.1.13.jar object_holder_definalize PLUGINSERVICE 
		/forge-1.16.4-35.1.13.jar runtime_enum_extender PLUGINSERVICE 
		/accesstransformers-2.2.0-shadowed.jar accesstransformer PLUGINSERVICE 
		/forge-1.16.4-35.1.13.jar capability_inject_definalize PLUGINSERVICE 
		/forge-1.16.4-35.1.13.jar runtimedistcleaner PLUGINSERVICE 
		/mixin-0.8.2.jar mixin TRANSFORMATIONSERVICE 
		/OptiFine_1.16.4_HD_U_G5_MOD.jar OptiFine TRANSFORMATIONSERVICE 
		/forge-1.16.4-35.1.13.jar fml TRANSFORMATIONSERVICE 
		/MixinBootstrap-1.0.5.jar mixinbootstrap TRANSFORMATIONSERVICE 
	FML: 35.1
	Forge: net.minecraftforge:35.1.13
	FML Language Providers: 
		javafml@35.1
		minecraft@1
	Mod List: 
		TreeChop-Mod-1.16.4.jar                           |treechop                      |treechop                      |0.7                 |DONE      |NOSIGNATURE
		Double-Doors-Mod-1.16.4.jar                       |Double Doors                  |doubledoors                   |2.1                 |DONE      |NOSIGNATURE
		Camels-Mod-1.16.4.jar                             |Camels Mod                    |camels                        |1.0.0               |DONE      |NOSIGNATURE
		Wyrmroost-1.16.3-1.2.9.jar                        |Wyrmroost                     |wyrmroost                     |1.16.3-1.2.9        |DONE      |NOSIGNATURE
		Spiders-2-Mod-1.16.4.jar                          |Spiders 2.0                   |spiderstpo                    |1.0.4               |DONE      |NOSIGNATURE
		jei-1.16.4-7.6.0.55.jar                           |Just Enough Items             |jei                           |7.6.0.55            |DONE      |NOSIGNATURE
		Doggy-Talents-Mod-1.16.4.jar                      |Doggy Talents 2               |doggytalents                  |2.0.1.1             |DONE      |NOSIGNATURE
		Macaws-Windows-Mod-1.16.4.jar                     |Macaw's Windows               |mcwwindows                    |1.0.2               |DONE      |NOSIGNATURE
		Vemerioraptor-Mod-1.16.4.jar                      |Vemerioraptor                 |vemerioraptor                 |1.16.4-1.0.0        |DONE      |NOSIGNATURE
		Space-Bosstools-1.16.4-3.5.jar                    |boss tools                    |boss_tools                    |3.3                 |DONE      |NOSIGNATURE
		BetterCaves-1.16.3-1.0.6.jar                      |YUNG's Better Caves           |bettercaves                   |1.16.3-1.0.6        |DONE      |NOSIGNATURE
		Waystones-Mod-1.16.4.jar                          |Waystones                     |waystones                     |7.3.1               |DONE      |NOSIGNATURE
		Placebo-1.16.4.jar                                |Placebo                       |placebo                       |4.3.3               |DONE      |NOSIGNATURE
		citadel-1.5.3.jar                                 |Citadel                       |citadel                       |1.5.3               |DONE      |NOSIGNATURE
		alexsmobs-1.2.1.jar                               |Alex's Mobs                   |alexsmobs                     |1.2.1               |DONE      |NOSIGNATURE
		Decorative-Blocks-Mod-1.16.4.jar                  |Decorative Blocks             |decorative_blocks             |1.6.2               |DONE      |NOSIGNATURE
		good-nights-sleep-1.16.4-1.2.9.jar                |Good Night's Sleep            |good_nights_sleep             |1.2.9               |DONE      |NOSIGNATURE
		Mutant-Beasts-Mod-1.16.4.jar                      |Mutant Beasts                 |mutantbeasts                  |1.16.4-1.1.3        |DONE      |d9:be:bd:b6:9a:e4:14:aa:05:67:fb:84:06:77:a0:c5:10:ec:27:15:1b:d6:c0:88:49:9a:ef:26:77:61:0b:5e
		u_team_core-1.16.4-3.1.17.191.jar                 |U Team Core                   |uteamcore                     |3.1.17.191          |DONE      |f4:a6:0b:ee:cb:8a:1a:ea:9f:9d:45:91:8f:8b:b3:ae:26:f3:bf:05:86:1d:90:9e:f6:32:2a:1a:ed:1d:ce:b0
		mcw-doors-1.0.1fix-mc1.16.4.jar                   |Macaw's Doors                 |mcwdoors                      |1.0.1               |DONE      |NOSIGNATURE
		Ice-and-Fire-Mod-1.16.4.jar                       |Ice and Fire                  |iceandfire                    |2.0.3-1.16.3        |DONE      |NOSIGNATURE
		Stupid-Horse-Stand-Still-Mod-1.16.4.jar           |Stupid Horse Stand Still      |horsestandstill               |1.16.3-1.0.1        |DONE      |1f:47:ac:b1:61:82:96:b8:47:19:16:d2:61:81:11:60:3a:06:4b:61:31:56:7d:44:31:1e:0c:6f:22:5b:4c:ed
		Immersive-Portals-Mod-1.16.4.jar                  |Immersive Portals             |immersive_portals             |0.7                 |DONE      |NOSIGNATURE
		forge-1.16.4-35.1.13-universal.jar                |Forge                         |forge                         |35.1.13             |DONE      |22:af:21:d8:19:82:7f:93:94:fe:2b:ac:b7:e4:41:57:68:39:87:b1:a7:5c:c6:44:f9:25:74:21:14:f5:0d:90
		Vending-Machine-Mod-1.16.4.jar                    |Vending Machine               |vm                            |1.0.0.3             |DONE      |NOSIGNATURE
		Lost-Trinkets-Mod-1.16.4.jar                      |Lost Trinkets                 |losttrinkets                  |0.1.5               |DONE      |NOSIGNATURE
		Scuba-Gear-Mod-1.16.4.jar                         |Scuba Gear                    |scuba_gear                    |1.0.1               |DONE      |NOSIGNATURE
		Supplementaries-Mod-1.16.4.jar                    |Supplementaries               |supplementaries               |0.9.15              |DONE      |NOSIGNATURE
		DynamicSurroundings-1.16.4-4.0.1.2.jar            |§3Dynamic Surroundings        |dsurround                     |1.16.4-4.0.1.2      |DONE      |b4:98:14:b9:76:55:25:4f:e5:5f:4d:71:90:87:43:5b:f9:d5:3a:02:60:42:5e:da:1f:15:9c:ff:be:a9:7c:77
		structure-gel-api-1.16.4-1.7.1.jar                |Structure Gel API             |structure_gel                 |1.7.1               |DONE      |NOSIGNATURE
		Corpse-Mod-1.16.4.jar                             |Corpse                        |corpse                        |1.16.4-1.0.0        |DONE      |NOSIGNATURE
		forge-1.16.4-35.1.13-client.jar                   |Minecraft                     |minecraft                     |1.16.4              |DONE      |NOSIGNATURE
		Farmers-Delight-Mod-1.16.4.jar                    |Farmer's Delight              |farmersdelight                |1.16.3-0.2.4b       |DONE      |NOSIGNATURE
		useful_backpacks-1.16.4-1.11.6.86.jar             |Useful Backpacks              |usefulbackpacks               |1.11.6.86           |DONE      |f4:a6:0b:ee:cb:8a:1a:ea:9f:9d:45:91:8f:8b:b3:ae:26:f3:bf:05:86:1d:90:9e:f6:32:2a:1a:ed:1d:ce:b0
		Beekeeper-Mod-1.16.4.jar                          |Beekeeper                     |bk                            |1.0.0.3             |DONE      |NOSIGNATURE
		Lollipop-Library-1.16.4.jar                       |Lollipop                      |lollipop                      |3.2.2               |DONE      |NOSIGNATURE
		Nifty-Mod-1.16.4.jar                              |Ornamental                    |ornamental                    |4.3.2               |DONE      |NOSIGNATURE
		curios-forge-1.16.4-4.0.3.0.jar                   |Curios API                    |curios                        |1.16.4-4.0.3.0      |DONE      |NOSIGNATURE
		Patchouli-Mod-1.16.4.jar                          |Patchouli                     |patchouli                     |1.16.2-47           |DONE      |NOSIGNATURE
		Xaeros_Minimap_20.29.1_Forge_1.16.4.jar           |Xaero's Minimap               |xaerominimap                  |20.29.1             |DONE      |NOSIGNATURE
		Carrots-Library-1.16.4.jar                        |Carrots Lib                   |carrots                       |3.0b1               |DONE      |NOSIGNATURE
		VanillaFoodPantry-Mod-1.16.4.jar                  |Vanilla Food Pantry           |vanillafoodpantry             |6.0b1               |DONE      |NOSIGNATURE
		Collective-Library-1.16.4.jar                     |Collective                    |collective                    |1.53                |DONE      |NOSIGNATURE
		Better-Weather-Mod-1.16.4.jar                     |Better Weather                |betterweather                 |1.0.1               |DONE      |NOSIGNATURE
		Extended-Lights-Mod-1.16.4.jar                    |Extended Lights               |extlights                     |3.3                 |DONE      |NOSIGNATURE
		AutoRegLib-1.16.4.jar                             |AutoRegLib                    |autoreglib                    |1.6-46              |DONE      |NOSIGNATURE
		Quark-Mod-1.16.4.jar                              |Quark                         |quark                         |r2.4-283            |DONE      |NOSIGNATURE
		Apotheosis-Mod-1.16.4.jar                         |Apotheosis                    |apotheosis                    |4.4.1               |DONE      |NOSIGNATURE
		Earth-Mobs-Mod-1.16.4.jar                         |Earth Mobs Mod                |earthmobsmod                  |1.16.4-0.1.2-Beta   |DONE      |NOSIGNATURE
		DoubleSlabs-1.16-3.4.10.jar                       |Double Slabs                  |doubleslabs                   |3.4.10              |DONE      |NOSIGNATURE
		obfuscate-0.5.1-1.16.3.jar                        |Obfuscate                     |obfuscate                     |0.5.1               |DONE      |e1:59:1a:56:ec:97:b3:d0:b3:4b:25:06:1f:83:b0:f4:fd:0c:24:e3:6d:ea:94:b1:9f:22:b0:38:13:60:88:ea
		EnigmaticLegacy-2.10.1.jar                        |Enigmatic Legacy              |enigmaticlegacy               |2.10.1              |DONE      |NOSIGNATURE
		The-Abyss-Project-Mod-1.16.4.jar                  |TheAbyss                      |theabyss                      |3.5.1               |DONE      |NOSIGNATURE
		Natures-Aura-Mod-1.16.4.jar                       |Nature's Aura                 |naturesaura                   |33.0                |DONE      |NOSIGNATURE
		furniture-7.0.0-pre19-1.16.3.jar                  |MrCrayfish's Furniture Mod    |cfm                           |7.0.0-pre19         |DONE      |NOSIGNATURE
		Productive-Bees-Mod-1.16.4.jar                    |Productive Bees               |productivebees                |1.16.4-0.5.2.1      |DONE      |NOSIGNATURE
		The-Undergarden-Mod-1.16.4.jar                    |The Undergarden               |undergarden                   |0.3.8               |DONE      |NOSIGNATURE
		Oh-The-Biomes-Youll-Go-Mod-1.16.4.jar             |Oh The Biomes You'll Go       |byg                           |1.1.1               |DONE      |NOSIGNATURE
		The-Bumblezone-Mod-1.16.4.jar                     |The Bumblezone                |the_bumblezone                |1.16.4-2.2.6        |DONE      |NOSIGNATURE
		Friendly-Fire-Mod-1.16.4.jar                      |FriendlyFire                  |friendlyfire                  |6.0.1               |DONE      |ea:45:b3:82:b6:9d:50:16:95:e7:2e:34:e1:92:d5:b4:9b:69:90:d3:4f:2e:71:99:b0:be:40:80:27:1f:3e:b0
		BetterMineshafts-Forge-1.16.3-1.1.1.jar           |YUNG's Better Mineshafts      |bettermineshafts              |1.16.3-1.1.1        |DONE      |NOSIGNATURE
		farlanders-1.16.4-1.3.6.jar                       |The Farlanders                |farlanders                    |1.3.6               |DONE      |NOSIGNATURE
	Crash Report UUID: 01d8c321-399a-4414-be7b-e2cfb6637ffc
	Patchouli open book context: n/a
	Launched Version: 1.16.4-forge-35.1.13
	Backend library: LWJGL version 3.2.2 build 10
	Backend API: AMD Radeon(TM) R6 Graphics GL version 4.5.13399 Compatibility Profile Context 15.201.1101.0, ATI Technologies Inc.
	GL Caps: Using framebuffer using OpenGL 3.0
	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'forge'
	Type: Client (map_client.txt)
	Graphics mode: fast
	Resource Packs: vanilla
	Current Language: English (US)
	CPU: 4x AMD A10-8700P Radeon R6, 10 Compute Cores 4C+6G
	OptiFine Version: OptiFine_1.16.4_HD_U_G5
	OptiFine Build: 20201106-171901
	Render Distance Chunks: 12
	Mipmaps: 4
	Anisotropic Filtering: 1
	Antialiasing: 0
	Multitexture: false
	Shaders: null
	OpenGlVersion: 4.5.13399 Compatibility Profile Context 15.201.1101.0
	OpenGlRenderer: AMD Radeon(TM) R6 Graphics
	OpenGlVendor: ATI Technologies Inc.
	CpuCount: 4

## Steps to Reproduce
1. All of the mods work until I put Optifine in the mods folder 


## OptiFine Version
Self-explanatory. 

## Installation Method
dropped it in the mods file

## Fabric/Forge Version
forge version 35.1.13



## Other Installed Mods
alexsmobs-1.2.1
Apotheosis-Mod-1.16.4
AutoRegLib-1.16.4
Beekeeper-Mod-1.16.4
BetterCaves-1.16.3-1.0.6
BetterMineshafts-Forge-1.16.3-1.1.1
Better-Weather-Mod-1.16.4
Camels-Mod-1.16.4
Carrots-Library-1.16.4
citadel-1.5.3
Collective-Library-1.16.4
Corpse-Mod-1.16.4
curios-forge-1.16.4-4.0.3.0
Decorative-Blocks-Mod-1.16.4
Doggy-Talents-Mod-1.16.4
Double-Doors-Mod-1.16.4
DoubleSlabs-1.16-3.4.10
DynamicSurroundings-1.16.4-4.0.1.2
Earth-Mobs-Mod-1.16.4
EnigmaticLegacy-2.10.1
Extended-Lights-Mod-1.16.4
farlanders-1.16.4-1.3.6
Farmers-Delight-Mod-1.16.4
Friendly-Fire-Mod-1.16.4
furniture-7.0.0-pre19-1.16.3
good-nights-sleep-1.16.4-1.2.9
Ice-and-Fire-Mod-1.16.4
Immersive-Portals-Mod-1.16.4
jei-1.16.4-7.6.0.55
Lollipop-Library-1.16.4
Lost-Trinkets-Mod-1.16.4
Macaws-Windows-Mod-1.16.4
mcw-doors-1.0.1fix-mc1.16.4
Mutant-Beasts-Mod-1.16.4
Natures-Aura-Mod-1.16.4
Nifty-Mod-1.16.4
obfuscate-0.5.1-1.16.3
Oh-The-Biomes-Youll-Go-Mod-1.16.4
Patchouli-Mod-1.16.4
Placebo-1.16.4
Productive-Bees-Mod-1.16.4
Quark-Mod-1.16.4
Scuba-Gear-Mod-1.16.4
Space-Bosstools-1.16.4-3.5
Spiders-2-Mod-1.16.4
structure-gel-api-1.16.4-1.7.1
Stupid-Horse-Stand-Still-Mod-1.16.4
Supplementaries-Mod-1.16.4
The-Abyss-Project-Mod-1.16.4
The-Bumblezone-Mod-1.16.4
The-Undergarden-Mod-1.16.4
TreeChop-Mod-1.16.4
u_team_core-1.16.4-3.1.17.191
useful_backpacks-1.16.4-1.11.6.86
VanillaFoodPantry-Mod-1.16.4
Vemerioraptor-Mod-1.16.4
Vending-Machine-Mod-1.16.4
Waystones-Mod-1.16.4
Wyrmroost-1.16.3-1.2.9
Xaeros_Minimap_20.29.1_Forge_1.16.4


## Log Files/Crash Reports
---- Minecraft Crash Report ----
// Surprise! Haha. Well, this is awkward.
 
Time: 12/26/20 1:05 PM
Description: Unexpected error
 
java.lang.NullPointerException: Unexpected error
	at net.minecraft.client.renderer.WorldRenderer.func_228441_a_(WorldRenderer.java:2205) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:structure_gel.mixins.json:WorldRendererMixin,pl:mixin:A}
	at net.minecraft.client.renderer.WorldRenderer.func_228426_a_(WorldRenderer.java:1594) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:structure_gel.mixins.json:WorldRendererMixin,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.func_228378_a_(GameRenderer.java:1022) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.redirect$zje000$redirectRenderingWorld(GameRenderer.java:2110) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.func_195458_a(GameRenderer.java:693) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
	at net.minecraft.client.Minecraft.func_195542_b(Minecraft.java:976) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:imm_ptl_mixins.json:client.MixinMinecraftClient,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinMinecraftClient_B,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:607) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:imm_ptl_mixins.json:client.MixinMinecraftClient,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinMinecraftClient_B,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:184) [?:?] {re:classloading,pl:runtimedistcleaner:A}
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_51] {}
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_51] {}
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_51] {}
	at java.lang.reflect.Method.invoke(Method.java:497) ~[?:1.8.0_51] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider.lambda$launchService$0(FMLClientLaunchProvider.java:51) [forge-1.16.4-35.1.13.jar:35.1] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider$$Lambda$500/1884982716.call(Unknown Source) [forge-1.16.4-35.1.13.jar:35.1] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:37) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:54) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:72) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:82) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:66) [modlauncher-8.0.6.jar:?] {}
 
 
A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------
 
-- Head --
Thread: Render thread
Stacktrace:
	at net.minecraft.client.renderer.WorldRenderer.func_228441_a_(WorldRenderer.java:2205) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:structure_gel.mixins.json:WorldRendererMixin,pl:mixin:A}
	at net.minecraft.client.renderer.WorldRenderer.func_228426_a_(WorldRenderer.java:1594) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:structure_gel.mixins.json:WorldRendererMixin,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.func_228378_a_(GameRenderer.java:1022) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
	at net.minecraft.client.renderer.GameRenderer.redirect$zje000$redirectRenderingWorld(GameRenderer.java:2110) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinGameRenderer_B,pl:mixin:APP:imm_ptl_mixins.json:client.render.MixinGameRenderer,pl:mixin:A}
-- Affected level --
Details:
	All players: 1 total; [ClientPlayerEntity['Oshertree'/376, l='ClientWorld minecraft:overworld', x=119.50, y=4.00, z=-54.50]]
	Chunk stats: Client Chunks (ImmPtl) 529
	Level dimension: minecraft:overworld
	Level spawn location: World: (128,4,-64), Chunk: (at 0,0,0 in 8,-4; contains blocks 128,0,-64 to 143,255,-49), Region: (0,-1; contains chunks 0,-32 to 31,-1, blocks 0,0,-512 to 511,255,-1)
	Level time: 102 game time, 102 day time
	Server brand: forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.world.ClientWorld.func_72914_a(ClientWorld.java:617) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,xf:fml:xaerominimap:xaero_clientworldclass,pl:mixin:APP:mixins.sndctrl.json:MixinClientWorld,pl:mixin:APP:betterweather.mixins.json:client.MixinClientWorld,pl:mixin:A}
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2024) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:imm_ptl_mixins.json:client.MixinMinecraftClient,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinMinecraftClient_B,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:628) [?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:imm_ptl_mixins.json:client.MixinMinecraftClient,pl:mixin:APP:imm_ptl_mixins.json:client.block_manipulation.MixinMinecraftClient_B,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:184) [?:?] {re:classloading,pl:runtimedistcleaner:A}
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:1.8.0_51] {}
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62) ~[?:1.8.0_51] {}
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:1.8.0_51] {}
	at java.lang.reflect.Method.invoke(Method.java:497) ~[?:1.8.0_51] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider.lambda$launchService$0(FMLClientLaunchProvider.java:51) [forge-1.16.4-35.1.13.jar:35.1] {}
	at net.minecraftforge.fml.loading.FMLClientLaunchProvider$$Lambda$500/1884982716.call(Unknown Source) [forge-1.16.4-35.1.13.jar:35.1] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:37) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:54) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:72) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:82) [modlauncher-8.0.6.jar:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:66) [modlauncher-8.0.6.jar:?] {}
 
 
-- System Details --
Details:
	Minecraft Version: 1.16.4
	Minecraft Version ID: 1.16.4
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_51, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 4057567680 bytes (3869 MB) / 6442450944 bytes (6144 MB) up to 6442450944 bytes (6144 MB)
	CPUs: 4
	JVM Flags: 9 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xss1M -Xmx6G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
	ModLauncher: 8.0.6+85+master.325de55
	ModLauncher launch target: fmlclient
	ModLauncher naming: srg
	ModLauncher services: 
		/mixin-0.8.2.jar mixin PLUGINSERVICE 
		/eventbus-3.0.5-service.jar eventbus PLUGINSERVICE 
		/forge-1.16.4-35.1.13.jar object_holder_definalize PLUGINSERVICE 
		/forge-1.16.4-35.1.13.jar runtime_enum_extender PLUGINSERVICE 
		/accesstransformers-2.2.0-shadowed.jar accesstransformer PLUGINSERVICE 
		/forge-1.16.4-35.1.13.jar capability_inject_definalize PLUGINSERVICE 
		/forge-1.16.4-35.1.13.jar runtimedistcleaner PLUGINSERVICE 
		/mixin-0.8.2.jar mixin TRANSFORMATIONSERVICE 
		/OptiFine_1.16.4_HD_U_G5_MOD.jar OptiFine TRANSFORMATIONSERVICE 
		/forge-1.16.4-35.1.13.jar fml TRANSFORMATIONSERVICE 
		/MixinBootstrap-1.0.5.jar mixinbootstrap TRANSFORMATIONSERVICE 
	FML: 35.1
	Forge: net.minecraftforge:35.1.13
	FML Language Providers: 
		javafml@35.1
		minecraft@1
	Mod List: 
		TreeChop-Mod-1.16.4.jar                           |treechop                      |treechop                      |0.7                 |DONE      |NOSIGNATURE
		Double-Doors-Mod-1.16.4.jar                       |Double Doors                  |doubledoors                   |2.1                 |DONE      |NOSIGNATURE
		Camels-Mod-1.16.4.jar                             |Camels Mod                    |camels                        |1.0.0               |DONE      |NOSIGNATURE
		Wyrmroost-1.16.3-1.2.9.jar                        |Wyrmroost                     |wyrmroost                     |1.16.3-1.2.9        |DONE      |NOSIGNATURE
		Spiders-2-Mod-1.16.4.jar                          |Spiders 2.0                   |spiderstpo                    |1.0.4               |DONE      |NOSIGNATURE
		jei-1.16.4-7.6.0.55.jar                           |Just Enough Items             |jei                           |7.6.0.55            |DONE      |NOSIGNATURE
		Doggy-Talents-Mod-1.16.4.jar                      |Doggy Talents 2               |doggytalents                  |2.0.1.1             |DONE      |NOSIGNATURE
		Macaws-Windows-Mod-1.16.4.jar                     |Macaw's Windows               |mcwwindows                    |1.0.2               |DONE      |NOSIGNATURE
		Vemerioraptor-Mod-1.16.4.jar                      |Vemerioraptor                 |vemerioraptor                 |1.16.4-1.0.0        |DONE      |NOSIGNATURE
		Space-Bosstools-1.16.4-3.5.jar                    |boss tools                    |boss_tools                    |3.3                 |DONE      |NOSIGNATURE
		BetterCaves-1.16.3-1.0.6.jar                      |YUNG's Better Caves           |bettercaves                   |1.16.3-1.0.6        |DONE      |NOSIGNATURE
		Waystones-Mod-1.16.4.jar                          |Waystones                     |waystones                     |7.3.1               |DONE      |NOSIGNATURE
		Placebo-1.16.4.jar                                |Placebo                       |placebo                       |4.3.3               |DONE      |NOSIGNATURE
		citadel-1.5.3.jar                                 |Citadel                       |citadel                       |1.5.3               |DONE      |NOSIGNATURE
		alexsmobs-1.2.1.jar                               |Alex's Mobs                   |alexsmobs                     |1.2.1               |DONE      |NOSIGNATURE
		Decorative-Blocks-Mod-1.16.4.jar                  |Decorative Blocks             |decorative_blocks             |1.6.2               |DONE      |NOSIGNATURE
		good-nights-sleep-1.16.4-1.2.9.jar                |Good Night's Sleep            |good_nights_sleep             |1.2.9               |DONE      |NOSIGNATURE
		Mutant-Beasts-Mod-1.16.4.jar                      |Mutant Beasts                 |mutantbeasts                  |1.16.4-1.1.3        |DONE      |d9:be:bd:b6:9a:e4:14:aa:05:67:fb:84:06:77:a0:c5:10:ec:27:15:1b:d6:c0:88:49:9a:ef:26:77:61:0b:5e
		u_team_core-1.16.4-3.1.17.191.jar                 |U Team Core                   |uteamcore                     |3.1.17.191          |DONE      |f4:a6:0b:ee:cb:8a:1a:ea:9f:9d:45:91:8f:8b:b3:ae:26:f3:bf:05:86:1d:90:9e:f6:32:2a:1a:ed:1d:ce:b0
		mcw-doors-1.0.1fix-mc1.16.4.jar                   |Macaw's Doors                 |mcwdoors                      |1.0.1               |DONE      |NOSIGNATURE
		Ice-and-Fire-Mod-1.16.4.jar                       |Ice and Fire                  |iceandfire                    |2.0.3-1.16.3        |DONE      |NOSIGNATURE
		Stupid-Horse-Stand-Still-Mod-1.16.4.jar           |Stupid Horse Stand Still      |horsestandstill               |1.16.3-1.0.1        |DONE      |1f:47:ac:b1:61:82:96:b8:47:19:16:d2:61:81:11:60:3a:06:4b:61:31:56:7d:44:31:1e:0c:6f:22:5b:4c:ed
		Immersive-Portals-Mod-1.16.4.jar                  |Immersive Portals             |immersive_portals             |0.7                 |DONE      |NOSIGNATURE
		forge-1.16.4-35.1.13-universal.jar                |Forge                         |forge                         |35.1.13             |DONE      |22:af:21:d8:19:82:7f:93:94:fe:2b:ac:b7:e4:41:57:68:39:87:b1:a7:5c:c6:44:f9:25:74:21:14:f5:0d:90
		Vending-Machine-Mod-1.16.4.jar                    |Vending Machine               |vm                            |1.0.0.3             |DONE      |NOSIGNATURE
		Lost-Trinkets-Mod-1.16.4.jar                      |Lost Trinkets                 |losttrinkets                  |0.1.5               |DONE      |NOSIGNATURE
		Scuba-Gear-Mod-1.16.4.jar                         |Scuba Gear                    |scuba_gear                    |1.0.1               |DONE      |NOSIGNATURE
		Supplementaries-Mod-1.16.4.jar                    |Supplementaries               |supplementaries               |0.9.15              |DONE      |NOSIGNATURE
		DynamicSurroundings-1.16.4-4.0.1.2.jar            |§3Dynamic Surroundings        |dsurround                     |1.16.4-4.0.1.2      |DONE      |b4:98:14:b9:76:55:25:4f:e5:5f:4d:71:90:87:43:5b:f9:d5:3a:02:60:42:5e:da:1f:15:9c:ff:be:a9:7c:77
		structure-gel-api-1.16.4-1.7.1.jar                |Structure Gel API             |structure_gel                 |1.7.1               |DONE      |NOSIGNATURE
		Corpse-Mod-1.16.4.jar                             |Corpse                        |corpse                        |1.16.4-1.0.0        |DONE      |NOSIGNATURE
		forge-1.16.4-35.1.13-client.jar                   |Minecraft                     |minecraft                     |1.16.4              |DONE      |NOSIGNATURE
		Farmers-Delight-Mod-1.16.4.jar                    |Farmer's Delight              |farmersdelight                |1.16.3-0.2.4b       |DONE      |NOSIGNATURE
		useful_backpacks-1.16.4-1.11.6.86.jar             |Useful Backpacks              |usefulbackpacks               |1.11.6.86           |DONE      |f4:a6:0b:ee:cb:8a:1a:ea:9f:9d:45:91:8f:8b:b3:ae:26:f3:bf:05:86:1d:90:9e:f6:32:2a:1a:ed:1d:ce:b0
		Beekeeper-Mod-1.16.4.jar                          |Beekeeper                     |bk                            |1.0.0.3             |DONE      |NOSIGNATURE
		Lollipop-Library-1.16.4.jar                       |Lollipop                      |lollipop                      |3.2.2               |DONE      |NOSIGNATURE
		Nifty-Mod-1.16.4.jar                              |Ornamental                    |ornamental                    |4.3.2               |DONE      |NOSIGNATURE
		curios-forge-1.16.4-4.0.3.0.jar                   |Curios API                    |curios                        |1.16.4-4.0.3.0      |DONE      |NOSIGNATURE
		Patchouli-Mod-1.16.4.jar                          |Patchouli                     |patchouli                     |1.16.2-47           |DONE      |NOSIGNATURE
		Xaeros_Minimap_20.29.1_Forge_1.16.4.jar           |Xaero's Minimap               |xaerominimap                  |20.29.1             |DONE      |NOSIGNATURE
		Carrots-Library-1.16.4.jar                        |Carrots Lib                   |carrots                       |3.0b1               |DONE      |NOSIGNATURE
		VanillaFoodPantry-Mod-1.16.4.jar                  |Vanilla Food Pantry           |vanillafoodpantry             |6.0b1               |DONE      |NOSIGNATURE
		Collective-Library-1.16.4.jar                     |Collective                    |collective                    |1.53                |DONE      |NOSIGNATURE
		Better-Weather-Mod-1.16.4.jar                     |Better Weather                |betterweather                 |1.0.1               |DONE      |NOSIGNATURE
		Extended-Lights-Mod-1.16.4.jar                    |Extended Lights               |extlights                     |3.3                 |DONE      |NOSIGNATURE
		AutoRegLib-1.16.4.jar                             |AutoRegLib                    |autoreglib                    |1.6-46              |DONE      |NOSIGNATURE
		Quark-Mod-1.16.4.jar                              |Quark                         |quark                         |r2.4-283            |DONE      |NOSIGNATURE
		Apotheosis-Mod-1.16.4.jar                         |Apotheosis                    |apotheosis                    |4.4.1               |DONE      |NOSIGNATURE
		Earth-Mobs-Mod-1.16.4.jar                         |Earth Mobs Mod                |earthmobsmod                  |1.16.4-0.1.2-Beta   |DONE      |NOSIGNATURE
		DoubleSlabs-1.16-3.4.10.jar                       |Double Slabs                  |doubleslabs                   |3.4.10              |DONE      |NOSIGNATURE
		obfuscate-0.5.1-1.16.3.jar                        |Obfuscate                     |obfuscate                     |0.5.1               |DONE      |e1:59:1a:56:ec:97:b3:d0:b3:4b:25:06:1f:83:b0:f4:fd:0c:24:e3:6d:ea:94:b1:9f:22:b0:38:13:60:88:ea
		EnigmaticLegacy-2.10.1.jar                        |Enigmatic Legacy              |enigmaticlegacy               |2.10.1              |DONE      |NOSIGNATURE
		The-Abyss-Project-Mod-1.16.4.jar                  |TheAbyss                      |theabyss                      |3.5.1               |DONE      |NOSIGNATURE
		Natures-Aura-Mod-1.16.4.jar                       |Nature's Aura                 |naturesaura                   |33.0                |DONE      |NOSIGNATURE
		furniture-7.0.0-pre19-1.16.3.jar                  |MrCrayfish's Furniture Mod    |cfm                           |7.0.0-pre19         |DONE      |NOSIGNATURE
		Productive-Bees-Mod-1.16.4.jar                    |Productive Bees               |productivebees                |1.16.4-0.5.2.1      |DONE      |NOSIGNATURE
		The-Undergarden-Mod-1.16.4.jar                    |The Undergarden               |undergarden                   |0.3.8               |DONE      |NOSIGNATURE
		Oh-The-Biomes-Youll-Go-Mod-1.16.4.jar             |Oh The Biomes You'll Go       |byg                           |1.1.1               |DONE      |NOSIGNATURE
		The-Bumblezone-Mod-1.16.4.jar                     |The Bumblezone                |the_bumblezone                |1.16.4-2.2.6        |DONE      |NOSIGNATURE
		Friendly-Fire-Mod-1.16.4.jar                      |FriendlyFire                  |friendlyfire                  |6.0.1               |DONE      |ea:45:b3:82:b6:9d:50:16:95:e7:2e:34:e1:92:d5:b4:9b:69:90:d3:4f:2e:71:99:b0:be:40:80:27:1f:3e:b0
		BetterMineshafts-Forge-1.16.3-1.1.1.jar           |YUNG's Better Mineshafts      |bettermineshafts              |1.16.3-1.1.1        |DONE      |NOSIGNATURE
		farlanders-1.16.4-1.3.6.jar                       |The Farlanders                |farlanders                    |1.3.6               |DONE      |NOSIGNATURE
	Crash Report UUID: 01d8c321-399a-4414-be7b-e2cfb6637ffc
	Patchouli open book context: n/a
	Launched Version: 1.16.4-forge-35.1.13
	Backend library: LWJGL version 3.2.2 build 10
	Backend API: AMD Radeon(TM) R6 Graphics GL version 4.5.13399 Compatibility Profile Context 15.201.1101.0, ATI Technologies Inc.
	GL Caps: Using framebuffer using OpenGL 3.0
	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'forge'
	Type: Client (map_client.txt)
	Graphics mode: fast
	Resource Packs: vanilla
	Current Language: English (US)
	CPU: 4x AMD A10-8700P Radeon R6, 10 Compute Cores 4C+6G
	OptiFine Version: OptiFine_1.16.4_HD_U_G5
	OptiFine Build: 20201106-171901
	Render Distance Chunks: 12
	Mipmaps: 4
	Anisotropic Filtering: 1
	Antialiasing: 0
	Multitexture: false
	Shaders: null
	OpenGlVersion: 4.5.13399 Compatibility Profile Context 15.201.1101.0
	OpenGlRenderer: AMD Radeon(TM) R6 Graphics
	OpenGlVendor: ATI Technologies Inc.
	CpuCount: 4


**DO NOT directly copy and paste log contents here on GitHub.**

## F3 Debug Screenshot
Minecraft's built-in debug screen provides *a lot* of useful information, and should be included even if the issue is not something that can be captured in a still image.

To open this menu, simply press `F3` on your keyboard while in-game. Please ensure the text is easily readable. Depending on the size/resolution of your monitor, you may have to adjust your GUI scale for all text to be completely visible on-screen.

## Prior Testing
If you've installed standalone:
- Does this happen in Vanilla without OptiFine?

If you've installed using Forge/Fabric:
- Does this happen without other mods installed?
yes
- Does this happen without any mods at all?
   - Only Forge/Fabric by itself.
   yes
- Does this happen in OptiFine standalone?
no
- Does this happen in Vanilla without OptiFine?
no
- Have you tried using a binary search to find which mods cause this issue?
   - To find conflicting mods, split your mods into 2 groups (not including OptiFine/OptiFabric, obviously). Remove one group, and test in-game. Keep the group that has the problem, and repeat until no more mods can be removed without the issue disappearing.
   - Does the issue still happen with only the remaining mods installed?
      - Forge/Fabric and remaining mods, without OptiFine

## Additional Information
Here goes any final remarks and everything else that might not fit in the previous sections.
