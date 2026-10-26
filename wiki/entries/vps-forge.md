# vps-forge

**Tags:** devops, vps, hardening, debian, ubuntu, skill
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2114681083308523617) · 2026-10-26
**Engagement:** roundup mention; repo ~28★ · 120-VM benchmark

## When to use
When you want an agent to set up and harden a Debian/Ubuntu VPS (SSH keys, firewall, fail2ban, Docker, TLS, backups, phone alerts) without locking you out—every risky change has an automatic undo window.

## What it does
Agent Skill for Claude Code, Codex, Cursor, Copilot, Gemini CLI and peers: ordered hardening with arm → change → new login → commit, or rollback. Author reports outside-in checklist scores rising substantially with the skill (e.g. production Docker box 79 → 99 across benchmarked runs).

## Recipe / links
- Repo: https://github.com/mountain-beaver/vps-forge (~28★)
- Skill: https://github.com/mountain-beaver/vps-forge/tree/main/skills/vps-forge
- Targets: Debian 12/13, Ubuntu 22.04/24.04/26.04
- Install: copy skill folder into your agent’s skills dir / follow repo quick start

## Why it made the cut
Full SKILL.md with safety-net workflow; clear VPS hardening use case; verifiable repo with CI, docs, and published benchmarks.
