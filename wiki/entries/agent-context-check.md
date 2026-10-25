# Agent-Context-Check — Broken Link Guard for SKILL.md

**Tags:** skill-authoring, qa, markdown, release, offline
**Source:** [@WhaleKim0](https://x.com/WhaleKim0/status/2112770816538816699) · 2026-10-21
**Engagement:** 2 likes / 0 reposts / 1 reply

## When to use
Before you **publish or ship** an agent skill — when the installer says “success” but referenced docs/scripts are missing (empty `docs/`, broken local Markdown links in `SKILL.md` / `AGENTS.md` / `CLAUDE.md`).

## What it does
Offline, zero-dependency checker for broken local Markdown links in agent context files. Catches “SKILL.md arrived, docs/ was empty” packaging failures before users hit them.

## Recipe / links
- Repo: https://github.com/oh79/agent-context-check
- Run it on the artifact users actually receive (installed skill tree), not only the source monorepo
- MIT, offline

## Why it made the cut
Born from a reproduced packaging bug; clear pre-release trigger; public MIT tool with a demo.
