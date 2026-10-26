# Oldhand 2.0 — Prove the work is done

**Tags:** quality-gates, verification, skill-pack, claude-code, cursor, codex
**Source:** [@berwin_singh](https://x.com/berwin_singh/status/2114579553301811256) · 2026-10-26
**Engagement:** discovery post (0 likes / 2 replies); repo ~7★

## When to use
When an agent claims a ticket or feature is finished and you want **scripts—not the model**—to decide done: plan → trace → smallest change → review → QA in the running app, with a ledger that refuses “done” while checks are missing, failing, or stale.

## What it does
Eleven portable `SKILL.md` skills (`oldhand` conductor plus build/contract/learn/plan/qa/rca/research/review/ship/trace). Works with Claude Code, Codex, Cursor, Copilot, Gemini CLI, and other hosts that read skills. Companion Python ledger scripts gate completion.

## Recipe / links
- Repo / site: https://github.com/berwinsingh/oldhand · https://berwinsingh.github.io/oldhand/
- Install (any agent): `npx skills add berwinsingh/oldhand --skill '*' -g`
- Claude plugin: `claude plugin marketplace add berwinsingh/oldhand` then `claude plugin install oldhand@oldhand`
- Needs Python 3.8+ for the three scripts; install the whole pack (stages share `ledger.py`)

## Why it made the cut
Concrete multi-skill pack with install paths, explicit “when to use,” and a non-LLM completion gate—not vibes-based “verify your work.”
