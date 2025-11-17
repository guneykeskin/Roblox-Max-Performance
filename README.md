## Roblox-Max-Performance

Do these:

```bash
Open Game Mode in settings.
Disable Memory Integerity in Windows Security.
Enable Hardware accelerated GPU scheduling.
```

Go to View advanced system settings and go to Advanced Tab, from there go to Performance and there in Visual Effects choose adjust for best performance.
Then go to Advanced Tab from there and go to Virtual Memory, from there untick the tick in the top and choose custom size and write Max and Min size as 16000.

Copy the path to the "RobloxPlayerBeta.exe", you can use Task Manager to do that.
Then go to the properties of that .exe and thick these:

```bash
Disable fullscreen optimizations
Run this program as an administator
```

Then in Graphics in Settings, click on "Add desktop app" and in the same path add that .exe file.
Then expand "Roblox Game Client" and set GPU preference to High Performance and Optimizations for windowed games to off.

Instal Process Lasso and these are the main settings to do/tick:

```bash
1. Main > Manage Processes of All Users
2. Main > Active Power Profile > Choose Highest Performance
3. Main > ProBalance Enabled
4. Options > General > Manage Processes of All Users
5. Options > General > Refresh Interval (GUI) > 5 seconds
6. Options > General > Refresh Interval (Governor) > 5 seconds
7. Options > CPU > ProBalance > Enable ProBalance
8. Options > CPU > ProBalance > Do Not Act on Foreground Process
9. Options > CPU > ProBalance > Do Not Act on Children of the Foreground Process
10. Options > CPU > ProBalance > Do Not Act on Processes of Non-Normal Priority
11. Options > CPU > ProBalance > Do Not Act on Services
12. Options > Power > Performance Mode > Change Power Profile when Engaged
13. Options > Power > Performance Mode > Enable Automatic Detection (e.g, Steam)
14. Options > Power > Performance Mode > Disable IdleSaver while Performance Mode Engaged
```

Then do these for Roblox:

```bash
CPU Priority > Always > Real Time
CPU Affinity > Always > None
I/O Priority > Always > High
GPU Priority > Always > Real Time
Memory Priority > Always > Normal
Exclude from ProBalance
Power Profile > Max Performance
```

Then go to the same folder where that .exe file is and add the folder named "ClientSettings" in that folder that is in this reporsity, here is what is inside:

```bash
{
  "FFlagHandleAltEnterFullscreenManually": "False",
  "FFlagMSRefactor5": "False",
  "FFlagDisablePostFx": "True",
  "FFlagRenderPostFx": "False",
  "FFlagDebugDisablePostFxV2": "True",
  "FFlagRenderAllParticles": "False",
  "FFlagRenderExplosionSmoke": "False",
  "FFlagRenderParticlesGPU": "False",
  "FFlagDebugSSAOForce": "False",
  "FIntSSAOMipLevels": "0",
  "FIntRobloxGuiBlurIntensity": "0",
  "DFIntAnimationLodFacsDistanceMin": "0",
  "DFIntAnimationLodFacsDistanceMax": "0",
  "DFIntAnimationLodFacsVisibilityDenominator": "0",
  "FStringPartTexturePackTablePre2022": "",
  "FStringTerrainMaterialTable2022": "",
  "FStringTerrainMaterialTablePre2022": "",
  "FIntDebugTextureManagerSkipMips": "-1",
  "DFIntDebugRestrictGCDistance": "1",
  "DFIntTextureCompositorActiveJobs": "0",
  "DFIntCSGLevelOfDetailSwitchingDistance": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0",
  "DFIntCSGv2LodsToGenerate": "0",
  "DFIntCSGv2LodMinTriangleCount": "0",
  "FIntTerrainArraySliceSize": "0",
  "DFIntDebugFRMQualityLevelOverride": "1",
  "FFlagDebugGraphicsDisableDirect3D11": "True",
  "DFFlagDebugPauseVoxelizer": "True",
  "FIntCSGVoxelizerFadeRadius": "0",
  "FFlagDebugGraphicsPreferVulkan": "True",
  "FFlagDebugForceFutureIsBrightPhase2": "True",
  "FFlagDebugForceFutureIsBrightPhase3": "True",
  "FFlagRenderFixFog": "True",
  "DFFlagFastEndUpdateLoop": "True",
  "DFIntGraphicsOptimizationModeMaxFrameTimeTargetMs": "1",
  "DFFlagEnableMeshPreloading2": "True",
  "FFlagDebugDeterministicParticles": "False",
  "FIntRomarkStartWithGraphicQualityLevel": "1",
  "FIntCameraFarZPlane": "1",
  "DFIntMaxMissedWorldStepsRemembered": "1",
  "FFlagEnableTerrainOptimizations": "True",
  "FFlagEnableTerrainFoliageOptimizations": "True",
  "DFIntRenderingThrottleDelayInMS": "1",
  "DFIntConnectionMTUSize": "1500",
  "DFIntWaitOnUpdateNetworkLoopEndedMS": "100",
  "FFlagFasterPreciseTime4": "True",
  "FFlagGameBasicSettingsFramerateCap": "True",
  "FFlagShaderLightingRefactor": "True",
  "FFlagRenderNoLowFrmBloom": "False",
  "DFIntAssemblyExtentsExpansionStudHendredth": "0",
  "FFlagDebugHumanoidRendering": "False",
  "DFFlagDebugRenderForceTechnologyVoxel": "False",
  "FFlagGlobalWindRendering": "False",
  "FFlagDebugDisableShadows": "True",
  "FIntRenderShadowIntensity": "0",
  "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
  "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
  "FIntRenderShadowmapBias": "1",
  "FIntDebugForceMSAASamples": "0",
  "FIntFRMMaxGrassDistance": "0",
  "FIntFRMMinGrassDistance": "0",
  "DFFlagTextureQualityOverrideEnabled": "True",
  "DFIntTextureQualityOverride": "0",
  "DFIntPerformanceControlTextureQualityBestUtility": "-1",
  "FIntTextureCompositorLowResFactor": "1",
  "DFFlagEnableRequestAsyncCompression": "True",
  "FFlagDebugSkyGray": "True",
  "FFlagCoreGuiTypeSelfViewPresent": "False",
  "FFlagTerrainDisableWaterRendering": "True",
  "DFFlagDebugGraphicsDisableTextures": "True",
  "FFlagRenderAtmosphere": "False",
  "FFlagRenderShadows": "False",
  "FFlagGraphicsFrameRateManager": "False",
  "DFIntTaskSchedulerTargetFps": "9999",
  "DFIntDebugSimulateFps": "0",
  "FFlagAdServiceEnabled": "False",
  "DFFlagDebugPerfMode": "True",
  "FIntRenderLocalLightUpdatesMax": "1",
  "FIntRenderLocalLightUpdatesMin": "1",
  "FIntRenderLocalLightFadeInMs": "0",
  "FFlagNewLightAttenuation": "True",
  "FFlagFastGPULightCulling3": "True",
  "FFlagDebugForceFSMCPULightCulling": "True",
  "DFIntMaxFrameBufferSize": "0",
  "FIntRenderGrassDetailStrands": "0",
  "FIntRenderGrassHeightScaler": "0",
  "FIntRuntimeMaxNumOfThreads": "2400",
  "FFlagDebugCheckRenderThreading": "True",
  "FFlagRenderDebugCheckThreading2": "True",
  "FFlagDebugRenderingSetDeterministic": "True",
  "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
  "DFIntCanHideGuiGroupId": "32380007",
  "DFFlagDisableDPIScale": "True",
  "FIntFontSizePadding": "4",
  "FLogNetwork": "7",
  "FFlagOptimizeNetwork": "True",
  "FFlagOptimizeNetworkRouting": "True",
  "FFlagOptimizeNetworkTransport": "True",
  "FFlagOptimizeServerTickRate": "True",
  "DFIntServerPhysicsUpdateRate": "60",
  "DFIntServerTickRate": "60",
  "FIntFullscreenTitleBarTriggerDelayMillis": "3600000",
  "FFlagDebugDisableTelemetryEphemeralCounter": "True",
  "FFlagDebugDisableTelemetryEphemeralStat": "True",
  "FFlagDebugDisableTelemetryEventIngest": "True",
  "FFlagDebugDisableTelemetryPoint": "True",
  "FFlagDebugDisableTelemetryV2Counter": "True",
  "FFlagDebugDisableTelemetryV2Event": "True",
  "FFlagDebugDisableTelemetryV2Stat": "True"
}
```

This makes the quality lowest possible and increases fps.

Then go to NVIDIA Control Panel and make sure to tick "Use the advanced 3D image settings" and click on "Take me there".
Then choose Program settings and open Roblox from there, here is all the settings:

```bash
1. Image Sharpening: Sharpening Off
3. Anisotropic filtering: Off
4. Antiailasing - FXAA: Off
5. Antiailasing - Gamma correction: Off
6. Antiailasing - Mode: Off
7. Antiailasing - Setting: None
8. Antiailasing - Transparency: Off
9. Background Application Max Frame Rate: Off
10. CUDA - GPUs: All
11. CUDA - Sysmem Fallback Policy: Driver Default
12. Low Latency Mode: Ultra
13. Max Frame Rate: Off
14. Multi-Frame Sampled AA (MFAA): Off
15. OpenGL GDI Compatibility: Auto
16. OpenGL rendering GPU: Auto-select
17. Power management mode: Prefer maximum performance
18. Texture filtering - Anistropic sample optimazation: On
19. Texture filtering - Negative LOD bias: Clamp
20. Texture filtering - Quality: High performance
21. Texture filtering - Trilinear optimization: On
22. Threaded optimization: On
23. Triple buffering: Off
24. Vertical sync: Off
25. Virtual Realiyu pre-rendered frames: 1
26. Vulkan/OpenGL present method: Auto
```

Next, press Win+R and write "appdata" and enter.
Then go to Local > Roblox folder.

Then edit GlobalBasicSettings_13.xml with notepad.
Then change these two:

```bash
<int name="FramerateCap">9999</int>
```

Then press CTRL+S to save the changes.
This will unlock your fps.

# Regedit

Press Win+R and write "regedit" then run it.

Here is everything that should be done:

```bash
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Power\PowerThrottling\PowerThrottlingOff = 1
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Multimedia\SystemProfile\NetworkThrottlingIndex = ffffffff
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Power\PowerSettings\54533251-82be-4824-96c1-47b60b740d00\0cc5b647-c1df-4637-891a-dec35c318583\Attributes = 0
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Multimedia\SystemProfile\Tasks\Games\Priority = 6, GPU Priority = 8, Scheduling Category = High, SFIO Priority = High
HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Microsoft\Direct3D\MaxPreRenderedFrames = 1
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Multimedia\SystemProfile\SystemResponsiveness = 10
```
