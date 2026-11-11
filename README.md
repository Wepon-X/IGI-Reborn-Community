# IGI: REBORN — Community Development Scaffold

> **Working title only.** This is an independent, IGI-inspired tactical FPS concept. It is not an official remake or an endorsed project.

## Project at a glance

A community-developed, single-player tactical first-person shooter concept focused on reconnaissance, infiltration, tense combat, readable enemy behaviour, and mission choice. The goal is a modular game optimized for modest Windows hardware.

| Area | Initial decision |
|---|---|
| Engine | Godot 4.x (pin an exact stable version after compatibility testing) |
| Renderer | Compatibility |
| First platform | Windows |
| Performance objective | 60 FPS at 1280×720, Low settings, Intel UHD 620 |
| Development laptop | 16 GB system RAM; exact CPU and memory configuration to be recorded |
| Architecture | Modular scenes, scripts, data resources, mission systems |
| Assets | Original, commissioned, public-domain, or appropriately licensed only |
| Collaboration | GitHub Issues, feature branches, pull requests, documented reviews |

**Performance note:** 60 FPS is a target, not a verified guarantee. Actual performance depends on CPU, cooling, memory configuration, drivers, scene complexity, and build settings. Profile exported builds on target hardware before making claims.

## Legal and naming notice — read before public promotion

This project is not affiliated with or endorsed by the rights holders of the original IGI games. The working title and franchise references are provisional. Do not use protected game branding, logos, characters, story material, maps, dialogue, music, sounds, models, textures, or other original assets without documented permission or a valid licence. Noncommercial/community intent does not itself grant permission.

Before public branding, distribution, fundraising, or release, obtain qualified IP review and any required permissions. If permission is unavailable, use a distinct original title, characters, setting, story, missions, and assets, and avoid implying an official connection. See [Legal & Asset Policy](docs/LEGAL_AND_ASSET_POLICY.md).

## Current status

**Pre-production / repository scaffold.** This repository does not yet contain a playable game, verified performance benchmark, or rights clearance.

## Quick start for contributors

1. Read [Contributing](CONTRIBUTING.md), [Game Design Document](docs/GDD.md), [Technical Design](docs/TECHNICAL_DESIGN.md), [Performance Targets](docs/PERFORMANCE_TARGETS.md), and [Legal & Asset Policy](docs/LEGAL_AND_ASSET_POLICY.md).
2. Check Issues and Discussions before starting substantial work.
3. Use the exact Godot version recorded in the technical design once the compatibility proof of concept pins it.
4. The Godot project will be added under `game/` during the prototype milestone; it is not present yet.
5. Keep contributions small, tested, and submitted through pull requests.

## Planned repository layout

```text
.
├── game/                  # Godot project, added during prototype sprint
│   ├── assets/
│   ├── data/
│   ├── scenes/
│   ├── scripts/
│   ├── shaders/
│   └── tests/
├── docs/
├── .github/
└── CONTRIBUTING.md
```

## Roadmap

See [Development Roadmap](docs/ROADMAP.md). Work begins with project governance and rights review, then a Compatibility-renderer performance proof of concept, core gameplay prototype, and one polished vertical slice.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md), use the issue and pull-request templates, and record asset provenance. A Code of Conduct and project licence should be adopted only after maintainer review; no licence is granted by this scaffold.

## Project decisions

See [Decision Log](docs/DECISIONS.md). Major engine, scope, naming, licensing, and architecture changes should be discussed before implementation.
