# Knighty Knight 2D

## Agent skills

Shared skills live in `.agents/skills/` (installed via `skills-lock.json`).

### Issue tracker

Issues live in GitHub Issues for `karthikgappiah/knighty-knight-2d` (via the `gh` CLI). See `docs/agents/issue-tracker.md`.

### Triage labels

Default vocabulary: `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`. See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: one `GLOSSARY.md` and `docs/adr/` at the repo root. See `docs/agents/domain.md`.

## Project state

Godot 4.7 2D game, freshly initialized: no scenes, scripts, main scene, or tests exist yet. `project.godot` is the only engine config. Update this file as architecture, commands, and test tooling get introduced.

## Engine configuration

- Renderer: GL Compatibility on all platforms (`project.godot` `[rendering]`). Avoid Forward+/Mobile-only features.
- Stretch mode `canvas_items`, aspect `expand`.
- Prefer editing `project.godot` through the Godot editor; hand edits are easy to get wrong.
- `.godot/` is an editor cache and is gitignored; never edit or commit it.

## Assets

`Assets/Tiny Swords (Free Pack)/` is a third-party art pack (Buildings, Particle FX, Terrain, UI Elements, Units). Treat it as read-only vendor content; Godot generates `.import` sidecars next to each file.
