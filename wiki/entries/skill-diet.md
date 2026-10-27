# skill-diet（给 Skill 减重）

**Tags:** meta, skill-authoring, token-budget, evaluation
**Source:** [@nicopreme](https://x.com/nicopreme/status/2114975730471997613) · 2026-10-27
**Also:** [@shao__meng](https://x.com/shao__meng/status/2115020426514469165) · [@Daviswh](https://x.com/Daviswh/status/2115040848886878216)
**Engagement:** ~250 bookmarks · ~189 likes · repo ~34★ · MIT

## When to use
When an existing skill is **bloated**, loads detail most tasks never need, or has **drifted** from the tool it teaches — or before you append another lesson to a SKILL.md.

## What it does
Meta-skill by Nico Bailon. Puts facts on the lowest load level (`description` → `SKILL.md` → `references/`), cuts what the model already knows, fixes stale tool names, then **keeps the slim version only if** the same tasks do at least as well with old / new / no skill. Author reports 70–80% fewer tokens with same results.

## Recipe / links
- Repo: https://github.com/nicobailon/skill-diet (~34★, MIT)
- Root `SKILL.md` + `references/diet.md` + `scripts/eval.mjs`
- Trigger: edit/diet a skill; after code changes that touch skill-described behavior

## Why it made the cut
Concrete installable meta-skill with an evaluation gate (not vibe-based deletion), clear maintenance use case, long-form author post + ZH rediscovery, verifiable repo.
