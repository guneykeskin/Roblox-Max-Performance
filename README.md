# Roblox-Max-Performance

Optimizations for Maximizing Roblox Performance

Copy the path to the "RobloxPlayerBeta.exe", you can use Task Manager to do that.
Then go to the properties of that .exe and thick these:

```bash
Disable fullscreen optimizations
Run this program as an administator
```

Then in Graphics in Settings, click on "Add desktop app" and in the same path add that .exe file.
Then expand "Roblox Game Client" and set GPU preference to High Performance and Optimizations for windowed games to off.

Then Install Process Lasso and do these for Roblox:

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
  "DFFlagDebugRenderForceTechnologyVoxel": "True",
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
  "DFIntMaxFrameBufferSize": "1",
  "FIntTerrainArraySliceSize": "0",
  "FIntRenderGrassDetailStrands": "0",
  "FIntRenderGrassHeightScaler": "0",
  "FIntRuntimeMaxNumOfThreads": "2400",
  "FFlagDebugCheckRenderThreading": "True",
  "FFlagRenderDebugCheckThreading2": "True",
  "FFlagDebugRenderingSetDeterministic": "True",
  "FFlagDebugDisableTelemetryEphemeralCounter": "True",
  "FFlagDebugDisableTelemetryEphemeralStat": "True",
  "FFlagDebugDisableTelemetryEventIngest": "True",
  "FFlagDebugDisableTelemetryPoint": "True",
  "FFlagDebugDisableTelemetryV2Counter": "True",
  "FFlagDebugDisableTelemetryV2Event": "True",
  "FFlagDebugDisableTelemetryV2Stat": "True"
}
```

This makes the quality lowest possible.

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
