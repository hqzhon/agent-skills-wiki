# Project Cairn（跨会话项目记忆）

**Tags:** knowledge-base, project-memory, skill, claude-code, codex
**Source:** [@DanKornas](https://x.com/DanKornas/status/2114619649446854829) · 2026-10-26
**Engagement:** 8 likes · 3 bookmarks · ~570 impressions; repo ~246★

## When to use
When project lessons keep dying between sessions or agent switches—you want decisions, pitfalls, progress and conclusions to live in the repo and only graduate to a long-term knowledge base after human confirmation.

## What it does
Agent skill that maintains `AGENTS.md`, `cairn/LOG.md`, `cairn/ROADMAP.md`, and per-topic notes during normal work. Agent can propose a “graduation” candidate; nothing hits the durable KB without your yes. Works with Claude Code and Codex.

## Recipe / links
- Repo: https://github.com/iBlinkQ/project-cairn (MIT, ~246★)
- Install: `npx skills add iBlinkQ/project-cairn --skill project-cairn -a claude-code` (or `-a codex`)
- Or: `git clone … ~/.claude/skills/project-cairn`

## Why it made the cut
Clear when-to-use for session amnesia; verifiable SKILL.md + scripts; solid community signal and open MIT repo.
