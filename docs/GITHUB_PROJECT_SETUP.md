# GitHub Project Setup

## Repository
- Keep the repository public only if the maintainer is comfortable with public visibility and community contributions.
- Protect `main`; require pull requests and at least one review when the team grows.
- Do not add a software licence until ownership and rights are reviewed.
- Enable Issues and Discussions; use milestones to group work.

## Suggested labels
- Type: `bug`, `enhancement`, `documentation`, `question`
- Status: `needs-triage`, `needs-discussion`, `ready`, `blocked`
- Area: `area-gameplay`, `area-ai`, `area-art`, `area-audio`, `area-performance`, `area-tools`

## Suggested milestones
- M0 — Project foundation and rights review
- M1 — Compatibility and performance proof of concept
- M2 — Core gameplay prototype
- M3 — Vertical slice
- M4 — Content production
- M5 — Release preparation

## Branching and review
Use `main` as the stable branch. Create short-lived branches such as `feature/player-controller`, `fix/ai-perception`, and `docs/contribution-guide`. Keep PRs focused, link issues, describe tests, and document asset provenance.

## First maintainer tasks
1. Confirm project naming and rights strategy.
2. Record target laptop CPU, OS build, GPU driver, and RAM configuration.
3. Pin and test an exact stable Godot 4.x version.
4. Establish a reproducible Windows export and benchmark scene.
5. Recruit a small founding team only after scope and review workflow are clear.
