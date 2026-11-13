# fuck-u-code-analysis（屎山体检 Skill）

**Tags:** code-quality, code-review, static-analysis, tech-debt
**Source:** [@huangho75845189](https://x.com/huangho75845189/status/2121085800360386987) · 2026-11-13

## When to use
Code changes are done and you want a quantitative quality check before committing or opening a PR (complexity, duplication, error handling, smells, tech debt) across 14 languages.

## What it does
Agent Skill bundled with Done-0/fuck-u-code (~7.3k★). The agent runs `fuck-u-code analyze`, gets a 0–100 overall score plus per-file scores across 7 dimensions / 11 metrics, then interprets them against the thresholds in the skill's references and prescribes specific refactors with structured review output.

## Recipe / links
- Repo: https://github.com/Done-0/fuck-u-code
- SKILL: `skills/fuck-u-code-analysis/SKILL.md`（+ `references/thresholds.md`）
- Prereq: `npm install -g eff-u-code`（Node ≥ 18），然后 `fuck-u-code analyze`

## Why it made the cut
Popular tool with a real tool-backed skill workflow and a clear pre-commit trigger; turns a static analyzer into an agent review step.
