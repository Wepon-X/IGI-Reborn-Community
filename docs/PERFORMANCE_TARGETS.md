# Performance Targets

These are engineering objectives, not measured claims or guarantees.

## Initial target
- Platform: Windows
- Resolution: 1280×720
- Preset: Low
- Reference GPU: Intel UHD 620
- Target frame rate: 60 FPS
- System RAM available: user's development laptop has 16 GB; exact CPU and memory configuration still to be recorded.

## Benchmark protocol
Record exact CPU, GPU driver, RAM configuration/channel mode, OS build, Godot version, renderer, resolution, graphics settings, scene, test duration, and capture method. Use exported builds, not only the editor.

Measure average FPS, 1% lows, frame time, peak RAM, CPU/GPU utilization where available, loading time, and thermal behaviour. Repeat runs after warm-up and report results honestly.

## Optimization priorities
- Compatibility renderer and conservative material/shader use.
- Baked/static lighting where appropriate; limit dynamic lights and shadow casters.
- Level of detail, occlusion culling, instancing, texture atlases, and compressed textures.
- Simple collision meshes and selective physics.
- Avoid costly global illumination, volumetrics, and ubiquitous real-time shadows until measured.
- Scale visual quality through presets.

## Acceptance
The prototype should remain stable and responsive on target hardware. If 60 FPS cannot be reached, profile bottlenecks and revise content/settings before changing the target. Never claim a benchmark without reproducible measurements.
