# Brotli Checker（Trail of Bits）

**Tags:** security, cve, brotli, trail-of-bits, skill
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2114681083308523617) · 2026-10-26
**Engagement:** roundup mention; repo ~52★ · official Trail of Bits skill

## When to use
When you need an agent to inventory potentially vulnerable Brotli decoder copies (source, deps, app packages, container filesystems) for CVE-2026-111497 and tell you which ones your app actually uses and how to update.

## What it does
Claude Code / Codex skill that scans for Brotli decoder fingerprints, investigates reachability (optionally with Trailmark for call graphs), and explains per-copy next steps. Can also run the scanner CLI without an agent (`brotli_inventory.py`).

## Recipe / links
- Repo: https://github.com/trailofbits/brotli-checker (~52★)
- Skill: https://github.com/trailofbits/brotli-checker/tree/main/skills/brotli-checker
- Install: copy `skills/brotli-checker` → `~/.claude/skills/` or `~/.codex/skills/`, or ask the agent to install from the GitHub path
- CLI: `python3 skills/brotli-checker/scripts/brotli_inventory.py /path/to/app`

## Why it made the cut
Concrete security skill with scripts from a known org; clear CVE remediation use case; verifiable MIT repo.
