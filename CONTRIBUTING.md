# Contributing

Thanks for helping build this independent tactical FPS project. The repository is in pre-production; no playable game is present yet.

## Before starting
- Read the README, GDD, Technical Design, Roadmap, and Legal & Asset Policy.
- Check existing Issues and open a discussion/issue before large changes.
- Pick a focused task and agree on its acceptance criteria with maintainers.

## Workflow
1. Create a branch from `main`: `feature/short-description`, `fix/short-description`, or `docs/short-description`.
2. Keep commits focused and use clear messages (e.g. `feat: add player movement prototype`).
3. Test in the pinned Godot version once established; document test steps and results.
4. Open a pull request using the template. Link related issues and include screenshots/video for visual changes.
5. Respond to review feedback; do not merge your own PR unless maintainers explicitly permit it.

## Code guidelines
- Prefer small, modular scenes, scripts, and data resources.
- Avoid hard-coded paths and unexplained magic numbers.
- Comment on non-obvious decisions, not every line.
- Profile before optimizing; report reproducible measurements.
- Do not commit generated imports, local settings, exports, secrets, or personal data.

## Assets and intellectual property
Only submit original, commissioned, public-domain, or appropriately licensed assets. Record source, creator, licence/version, attribution, modifications, and permitted uses in `docs/ASSET_MANIFEST_TEMPLATE.csv`. Never submit ripped game assets or content with unclear provenance. Read the legal policy before contributing art, audio, story, or branding.

## Pull request checklist
- [ ] Scope is focused and linked to an issue where appropriate.
- [ ] Tests or manual verification are described.
- [ ] No unrelated generated files or secrets.
- [ ] Asset provenance and licence are documented.
- [ ] Documentation is updated where needed.
