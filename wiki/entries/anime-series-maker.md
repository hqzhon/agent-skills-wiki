# Anime Series Maker

**Tags:** video, anime, remotion, renoise, skill, series
**Source:** [@Mayz1169](https://x.com/Mayz1169/status/2114715882215915804) · 2026-10-26
**Engagement:** author reply · repo early (few ★) · MIT · Agent Skill + Renoise MCP

## When to use
When you want a **recurring anime cast** (not one-off clips): give 2 character sheets + one story line and have Claude Code / Codex run hook → shot script → voiced clips → QA → edit → Instagram-safe cover/caption as a skill.

## What it does
Series bible in `series.json` (cast, style, voices, locations, gags) so later episodes stay on-model. Hook pitches from view-ranked formulas; per-second shot lists; `build_prompt.py` validates sheets/cameras/timings before spend; cost gate + first-clip check before batch; per-clip QA vs sheets. Packaged as `skills/anime-series-maker` SKILL.md for coding agents, powered by Renoise MCP.

## Recipe / links
- Repo: https://github.com/Mayzmei/anime-series-maker
- Skill folder: `skills/anime-series-maker` (see README EN / 简体中文)
- Needs Renoise MCP + agent that loads Agent Skills

## Why it made the cut
Executable SKILL.md workflow with validation/cost gates and a clear series use-case — more than a prompt dump, even while stars are still low.
