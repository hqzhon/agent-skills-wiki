# Superpowers (obra)

**Tags:** skill-pack, methodology, tdd, brainstorming, planning
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2114530319349248402) · 2026-10-26
**Engagement:** 0 likes / 1 reply on this hour’s brainstorming tip (pack is widely installed; repo ~305k★)

## When to use
When you want a coding agent to follow a **full delivery loop** instead of jumping straight into code: clarify requirements (`brainstorming`), write a plan, run true red→green→refactor TDD (`test-driven-development`), dispatch subagents, request/receive review, and verify before claiming done. Load for new features, fuzzy requirements, bug fixes, and refactors.

## What it does
Composable Agent Skills framework + methodology (MIT). Skills auto-trigger: brainstorm → design sign-off → implementation plan → subagent-driven development with TDD and verification. Highlighted this hour: `brainstorming` (small changes ask the critical gap; large tasks list options and wait) and `test-driven-development` (RED must fail for missing behavior, then minimal GREEN).

## Recipe / links
- Repo: https://github.com/obra/superpowers (~305k★, MIT)
- Brainstorming SKILL: https://github.com/obra/superpowers/blob/main/skills/brainstorming/SKILL.md
- TDD SKILL: https://github.com/obra/superpowers/blob/main/skills/test-driven-development/SKILL.md
- Install (examples): Claude `/plugin install superpowers@claude-plugins-official`; Codex App → Plugins → Coding → Superpowers; see README for Cursor / Gemini / Copilot / etc.
- Other skills in pack: writing-plans, executing-plans, systematic-debugging, subagent-driven-development, verification-before-completion, …

## Why it made the cut
Concrete installable skills with when-to-use + verification steps in the source posts, plus a large public SKILL.md pack—not empty “use TDD” advice.
