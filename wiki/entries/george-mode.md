# george-mode（决策闭环 skill 包）

**Tags:** skill-pack, decision-loop, verification, quality-gates
**Source:** [@George_ONair](https://x.com/George_ONair/status/2114624526793441621) · 2026-10-26
**Engagement:** 2 likes · 23 impressions (discovery); repo MIT

## When to use
When you want agents to run a **decide → act → verify → reflect** loop: register goals, assumptions, falsifiers and stop conditions before high-stakes choices, and show evidence before claiming "done".

## What it does
11 bilingual (zh/en) skills: `george-mode` router plus investigate / decide / design / engineer / evaluate / orchestrate / deliver / verify / reflect / resume. Installer symlinks into `~/.agents/skills`, Claude Code, Codex, Cursor, Gemini, OMP. Engineering playbooks adapted from pstack (MIT).

## Recipe / links
- Repo: https://github.com/qingsongcui/george-mode-skills (MIT)
- Install: `python3 scripts/install.py --apply` (or symlink `skills/george-*` into `~/.claude/skills/`)
- Skills dir: `skills/george-*` (11× SKILL.md)

## Why it made the cut
Concrete open-source skill pack with clear decision/verify use cases; verifiable SKILL.md layout and install script; bilingual docs.
