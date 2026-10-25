# Codebase-Health — Maintainability Audit + Fix PRs

**Tags:** code-quality, dry, ci, maintenance, claude-code
**Source:** [@arklanq](https://x.com/arklanq/status/2112961549975310390) · 2026-10-21
**Engagement:** 3 likes / 0 reposts / 1 reply

## When to use
After agents have been shipping fast and you suspect the repo is getting expensive to maintain — god files, DRY violations, flaky tests, stale CI/deps, dead code, leftover agent notes.

## What it does
Agent skill that scans for common health problems, then opens PRs with the fixes you approve (rather than silently rewriting everything).

## Recipe / links
- Install: `npx skills add arklanq/agent-skills`
- Run the codebase-health skill on a repo you maintain
- Review proposed PRs before merge

## Why it made the cut
Concrete install command + named failure modes + PR-based remediation loop = reusable recipe with a clear trigger.
