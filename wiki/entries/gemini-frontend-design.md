# gemini-frontend-design（Google Gemini 官方）

**Tags:** frontend, web-design, ui, official
**Source:** [@GreatCreations_](https://x.com/GreatCreations_/status/2121052386525618230) · 2026-11-13

## When to use
Building or redesigning a website / web app and you want the agent to commit to a tailored visual direction (layout, color, typography, custom imagery, motion) instead of generic template UI.

## What it does
Official Google Gemini skill from `google-gemini/demolab`. It pushes the agent to derive the aesthetic from the subject's real materials and audience, sustain the craft across the page, and visually verify the rendered page before finishing. Ships plugin manifests for Claude Code, Codex and Cursor. The post cites Google saying users preferred designs made with it 67% of the time vs. no skill (Google's claim, not independently verified).

## Recipe / links
- Repo: https://github.com/google-gemini/demolab (Apache-2.0)
- SKILL: `skills/gemini-frontend-design/SKILL.md`
- Install: `npx skills add google-gemini/demolab --skill gemini-frontend-design`（或用仓库内的 Claude/Codex/Cursor plugin manifest）

## Why it made the cut
Official vendor skill with a real SKILL.md, a clear trigger, and multi-agent packaging; complements Taste Skill / Impeccable in the frontend-design space.
