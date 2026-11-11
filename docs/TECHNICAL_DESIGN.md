# Technical Design

## 1. Engine and platform
Use Godot 4.x with the Compatibility renderer as the initial candidate. Pin an exact stable version only after testing project import, Windows export, input, navigation, and rendering on target hardware. Windows is the first platform.

## 2. Project structure
Keep systems modular and data-driven. Planned layout:
```text
game/
  assets/{audio,materials,models,textures,ui}
  data/{missions,weapons,enemies}
  scenes/{levels,player,weapons,enemies,ui}
  scripts/{core,player,combat,ai,missions,ui}
  shaders/
  tests/
```
Do not add empty project files that imply a runnable game before the prototype exists.

## 3. Player
Use `CharacterBody3D` for predictable first-person movement. Separate input mapping, movement state, camera, interaction, weapon handling, and health/damage. Expose tunable values through exported properties or resources.

## 4. Weapons
A weapon scene owns presentation and firing behaviour; a data resource defines tuning. Separate hit detection, damage application, ammunition, reload, and effects. Begin with ray-based hitscan where suitable; add projectile simulation only when gameplay requires it.

## 5. Enemy AI
Use `NavigationAgent3D` for path following and a finite-state machine for explicit states, with small utility scores for tactical action selection. Perception produces observations; communication shares observations; decision logic consumes them. Throttle distant/inactive AI updates and profile navigation costs.

## 6. Mission system
Represent objectives and extraction conditions as data-driven resources/nodes. Mission state must be testable without depending on UI. Use signals/events to notify HUD and audio.

## 7. Audio perception
Publish sound events with position, category, and strength. AI evaluates events according to hearing range and obstruction approximation. Avoid expensive acoustic simulation in the first prototype.

## 8. Save/configuration
Use versioned save structures. Store user settings separately from campaign progress. Handle missing or older fields safely.

## 9. Rendering and optimization
Prefer baked/static lighting where possible. Use LOD, occlusion culling, instancing, texture atlases, and compressed textures. Limit dynamic lights and shadow casters. Avoid costly global illumination, volumetrics, and heavy screen-space effects until measured.

## 10. Testing and build workflow
1. Open the project in the pinned Godot version.
2. Run smoke tests for main scene, input, and loading.
3. Test movement, weapon, AI perception, objective state, and extraction.
4. Export a Windows build and test it on target hardware.
5. Record hardware, driver, resolution, settings, scene, and measurement method with each benchmark.

## 11. Initial acceptance criteria
- Project opens without import/parse errors in pinned engine.
- Main prototype scene loads and can be completed.
- Core systems can be tested independently.
- No unlicensed assets or undocumented dependencies are committed.
- Performance results include reproducible hardware and settings details.
