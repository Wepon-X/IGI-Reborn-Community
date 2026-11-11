# Development Roadmap

Dates and staffing are intentionally not promised until contributor capacity is known.

## M0 — Project foundation and rights review
- Confirm ownership, governance, repository workflow, and contributor process.
- Obtain IP review for the working title and franchise references.
- Decide whether to proceed under an authorized licence or use a distinct original identity.
- Choose a project licence only after reviewing code and asset rights.
- Pin a tested Godot 4.x stable version.
**Exit:** written governance and legal/asset policy; repository workflow ready.

## M1 — Compatibility and performance proof of concept
- Create minimal Godot Compatibility project.
- Test Windows export on Intel UHD 620.
- Build a small outdoor/indoor test area and controllable player.
- Test lighting, materials, textures, and a small number of AI agents.
- Capture reproducible FPS, frame-time, memory, and stability results.
**Exit:** benchmark report and decision to proceed, optimize, or revise scope.

## M2 — Core gameplay prototype
- Player movement and camera.
- One weapon with aim, fire, reload, recoil, and audio.
- Interaction and objective framework.
- One basic enemy with patrol, perception, investigation, and combat states.
**Exit:** short playable loop with clear feedback.

## M3 — Vertical slice
- One original/licensed mission environment with multiple routes.
- Enemy communication and search behaviour.
- Extraction and mission results.
- Basic HUD, settings, subtitles, and accessibility foundations.
- Profiling and QA on target hardware.
**Exit:** polished, complete, repeatable mission demonstrating design pillars.

## M4 — Content production
Expand original environments, mission definitions, characters, animations, weapons, audio, and narrative. Add QA automation and asset validation.

## M5 — Release preparation
Complete legal/licence audit, Windows packaging, save migration, crash handling, external playtesting, accessibility review, and final quality sign-off.

## First tasks
1. Record exact CPU, Windows build, RAM configuration, and graphics driver.
2. Install a candidate stable Godot 4.x version and verify Compatibility renderer.
3. Create a minimal project and Windows export.
4. Establish a baseline benchmark scene and log.
5. Add player movement and camera.
