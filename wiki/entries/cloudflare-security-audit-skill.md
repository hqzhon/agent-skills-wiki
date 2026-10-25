# Cloudflare Security Audit Skill

**Tags:** security, audit, cloudflare, claude-code, cursor, multi-phase
**Source:** [@tungoldshou](https://x.com/tungoldshou/status/2114323679517737360) · 2026-10-25
**Engagement:** 2 likes / 1 repost / 3 replies / 1 bookmark

## When to use
When you want a coding agent to run a **structured, multi-phase security audit** on your own repos and produce findings you can independently verify (not rubber-stamp).

## What it does
Agent-agnostic skill (originally from Cloudflare) that walks cloud/deploy config, CI supply chain, data isolation, and LLM-specific issues across ~6 phases. Outputs machine-readable, independently verifiable findings for Claude Code, Codex, or Cursor.

## Recipe / links
- Repo: https://github.com/cloudflare/security-audit-skill
- Install into Claude Code / Cursor / Codex
- Run on a repo you own; review every finding before acting
- Related discussion: multi-phase structure noted in Chinese thread [@xjtumj](https://x.com/xjtumj/status/2113599178517647664)

## Why it made the cut
Concrete GitHub skill with a clear audit workflow, official Cloudflare provenance, and repeated independent mentions in the scan window.
