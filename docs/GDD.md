# Game Design Document (GDD)

**Status:** Draft 0.1 — a working design, not a final content commitment.

## 1. Vision
Create a tense, single-player tactical FPS inspired by broad design principles of classic military espionage games: isolation, reconnaissance, infiltration, careful resource use, dangerous opponents, and readable spaces. The project must stand on its own through original worldbuilding, characters, missions, art, audio, and writing.

## 2. Design pillars
1. **Reconnaissance before action:** observe patrols, identify threats, and plan routes.
2. **Meaningful tactical freedom:** multiple viable routes and approaches; stealth and direct combat both supported, with consequences.
3. **Credible opposition:** enemies coordinate but have imperfect information and can be misled.
4. **Readable realism:** animation, audio, weapons, and environments communicate useful gameplay information.
5. **Accessible performance:** scalable settings and careful content budgets.
6. **Replayable missions:** optional objectives, alternate routes, and varied approaches.

## 3. Player loop
**Observe → plan → infiltrate → adapt → complete objective → extract → review.**
Players make decisions about timing, visibility, noise, ammunition, equipment, and risk.

## 4. Setting and story
The setting, factions, plot, character names, dialogue, mission events, and visual identity must be original or appropriately licensed. Do not copy original IGI plotlines, dialogue, maps, biographies, or other protected expression. Any franchise-specific use requires rights-holder permission and legal review.

## 5. First playable mission
The first milestone is one polished vertical-slice mission, not a full campaign. Include:
- One compact outdoor-to-indoor environment.
- A clear primary objective and extraction.
- At least two viable routes.
- A small set of patrols and enemy response states.
- Optional information or equipment objective.
- Complete start-to-finish loop with restart and success/failure feedback.

## 6. Player mechanics
Prototype in this order: walk/run/sprint/crouch/prone; camera look and aiming; weapon sway/recoil; interaction and objectives; inventory/ammunition/reload. Add advanced traversal only when the core loop is stable.

## 7. Weapons and equipment
Start with three functional weapon archetypes. Define behaviour in data resources: rate of fire, spread, recoil, reload duration, magazine capacity, damage model, audio, and animation references. Use original designs and licensed audio/visual content.

## 8. Stealth and detection
Detection may consider line of sight, distance, lighting/cover abstraction, movement, and sound. Give players feedback through enemy posture, voice/radio cues, and restrained UI indicators. Sound events should use a common event interface.

## 9. Enemy behaviour
Initial awareness states: Unaware, Suspicious, Investigating, Alert, Combat, Searching/Returning to patrol. Enemies may share observations but must not know the player's exact location without evidence.

## 10. Mission design
Each mission defines start/extraction conditions, primary/optional objectives, patrols, navigation/interactions, fail conditions, recovery rules, and performance test cases.

## 11. UI and accessibility
Provide remappable controls, adjustable sensitivity, subtitles, scalable HUD, audio sliders, graphics presets, and clear difficulty options. Use colour-independent indicators and readable text.

## 12. Non-goals for the first prototype
Full campaign, multiplayer/live services, large vehicle simulation, huge open world, destructive-everything physics, and unlicensed franchise assets.
