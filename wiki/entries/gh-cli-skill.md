# gh — GitHub CLI 官方 Agent Skill

**Tags:** github, cli, gh, official, devtools
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2121098893643645182) · 2026-11-13

## When to use
An agent drives the GitHub CLI (`gh`) and you want correct structured output, pagination, repo targeting, search-vs-list choices and `gh api` fallbacks instead of guesswork.

## What it does
Official skill shipped inside `cli/cli`. Covers non-interactive behavior, `--json`/`--jq`/`--template` parsing, the default 30-item caps and `-L`, `gh api --paginate`, GraphQL `totalCount`, and flag collisions like `-T`. The post also shows the safe-install habit: preview the SKILL.md read-only before installing.

## Recipe / links
- SKILL: https://github.com/cli/cli/blob/trunk/skills/gh/SKILL.md
- Preview (read-only): `gh skill preview cli/cli skills/gh/SKILL.md`
- Read the full SKILL.md and sibling files before installing; check source, permissions and dependencies

## Why it made the cut
First-party skill from the GitHub CLI maintainers, concrete and verifiable, useful for almost any coding agent that touches GitHub.
