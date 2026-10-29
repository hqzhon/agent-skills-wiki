# baoyu-design（本地 Claude Design / Slides / Dashboard）

**Tags:** design, slides, dashboard, html, skill-pack, chinese
**Source:** [@dotey](https://x.com/dotey/status/2115667965328977920) · 2026-10-29
**Engagement:** ~4.7k★ · MIT · v2 ships Design + Slides + Dashboard as local Agent Skills

## When to use
When you want **Claude Design / Slides / Dashboard**-class UI mockups, decks, and data dashboards **inside Cursor / Claude Code / Codex** as self-contained HTML—without claude.ai Artifacts or uploading files to the web UI.

## What it does
Portable Agent Skill pack (MIT) that repackages Claude Design methodology for local agents. Produces hi-fi UI, interactive prototypes, wireframes, landing pages, mobile screens, slide decks, and dashboards under `designs/`. Companion skills `claude-slides`, `claude-design`, `claude-design-system`, and `claude-dashboard` write typed project folders and open local editors (`artifact.mjs`). Supports design-system import (incl. offline `.fig`), PPTX export, and point-and-edit preview loops.

## Recipe / links
- Repo: https://github.com/JimLiu/baoyu-design (~4.7k★, MIT)
- Install: `npx skills add JimLiu/baoyu-design` (optional `-g` / `--agent cursor|claude-code|codex`)
- Skills: `skills/baoyu-design/SKILL.md` plus `skills/claude-{slides,design,design-system,dashboard}/`
- Best with a strong model (README recommends Opus-class)

## Why it made the cut
Clear when-to-use, runnable SKILL.md pack with install CLI, verifiable MIT repo, and high community signal on the v2 launch post—not a taste rant or closed demo.
