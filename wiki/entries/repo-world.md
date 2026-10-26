# Repo World

**Tags:** onboarding, visualization, gamedev, claude-skill
**Source:** [@AJerrary](https://x.com/AJerrary/status/2114540323166986537) · 2026-10-26
**Engagement:** 1 like / 1 reply (discovery post; repo ~1★)

## When to use
When the user wants to **explore, visualize, gamify, or onboard onto a codebase**—“turn my repo into a game”, “repo world”, “make onboarding fun”, `/repo-world`. Not for production refactors; for understanding structure and teaching the map.

## What it does
Claude skill: deterministic `scan.py` → optional Claude lore → `build.py` → single offline HTML RPG. Folders become districts, classes NPCs, huge files bosses, import cycles rifts, deleted files graveyard.

## Recipe / links
- Repo: https://github.com/OutOfAmine/repo-world (MIT)
- Skill: `SKILL.md` at repo root
- Demo: https://outofamine.github.io/repo-world/
- Flow: `python3 scripts/scan.py <repo> -o world.json` → write `lore.json` → `python3 scripts/build.py world.json -l lore.json -o repo-world.html`

## Why it made the cut
Installable SKILL.md with explicit when-to-use, scripts, and a playable demo—more than a vibe tweet.
