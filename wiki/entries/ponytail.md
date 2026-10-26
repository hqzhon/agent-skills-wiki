# Ponytail（lazy senior dev）

**Tags:** coding-style, yagni, skill-pack, claude-code
**Source:** [@xd1309007813404](https://x.com/xd1309007813404/status/2114551919310237993) · 2026-10-26
**Engagement:** 1 like / 4 replies (discovery post; repo ~176K★)

## When to use
When the user wants the agent to **write the smallest complete change**—complains about over-engineering, says “be lazy”, “simplest solution”, “yagni”, or “ponytail”, or the task is ordinary coding/fix/refactor/review where bloat is a risk. Levels: lite / full (default) / ultra.

## What it does
A portable Agent Skill (`skills/ponytail/SKILL.md` + `AGENTS.md`) that installs a decision ladder: skip features nobody asked for → reuse existing code → stdlib/platform → installed deps → one-liner → minimum new code. Keeps validation, security, accessibility, and data-loss handling. Ends replies with what was skipped and residual risk.

## Recipe / links
- Repo: https://github.com/DietrichGebert/ponytail (~176K★, MIT)
- Site: https://ponytail.dev/
- Claude Code: `/plugin marketplace add DietrichGebert/ponytail` then `/plugin install ponytail@ponytail`
- Skills CLI: `npx skills add DietrichGebert/ponytail`
- Switch intensity: `/ponytail lite|full|ultra|off`

## Why it made the cut
Concrete SKILL.md with clear when-to-use, multi-agent install docs, and a verifiable public repo—not empty “write less code” advice.
