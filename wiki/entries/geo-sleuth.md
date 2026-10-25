# Geo-Sleuth — Photo Geolocation Agent Skill

**Tags:** geolocation, vision, openstreetmap, osint, claude-code, cursor
**Source:** [@KowalPrato4o](https://x.com/KowalPrato4o/status/2112099689071849672) · 2026-10-19
**Engagement:** 0 likes / 0 reposts / 2 replies (citing [@Dinosn](https://x.com/Dinosn/status/2111682739342864783): 288 likes / 40 reposts / 15 replies / 310 bookmarks)

## When to use
When you need an agent to figure out **where a photo was taken** from visual cues alone (no EXIF/GPS) — bridge, ridge, skyline, street view — and show its reasoning.

## What it does
Packages OpenStreetMap geometry, elevation skylines, satellite imagery, and street view into a reusable agent skill. Compatible with Claude Code, Codex, Cursor, Gemini CLI, OpenCode, and GitHub Copilot. README case: bridge + mountain only → location within ±2 m.

## Recipe / links
- Repo: https://github.com/Oldcircle/geo-sleuth
- Drop the skill into a compatible agent host and ask it to geolocate a photo
- Prefer photos with distinctive terrain/structures; expect a chain-of-evidence writeup, not a single pin with no rationale

## Why it made the cut
Concrete SKILL.md/repo, clear trigger (photo → place), strong community signal on the upstream share, and multi-host evidence of use.
