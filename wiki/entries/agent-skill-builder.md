# agent-skill-builder（会“失败”的 Skill 生成器）

**Tags:** meta-skill, skill-authoring, validation, claude-code
**Source:** [@ConorBronsdon](https://x.com/ConorBronsdon/status/2121045408692736007) · 2026-11-13

## When to use
You're writing new skills and want spec-current frontmatter for Claude Code or the portable Agent Skills core, with a validator that actually fails broken skills and detects drift.

## What it does
A skill that builds skills: from a plain-language description it picks runtime (Claude Code extensions vs. portable core) and shape (reference, bounded task, tool-backed workflow), then validates each runtime separately. Its test suite includes deliberately invalid skills, and it checks the live Claude Code field set weekly. It checks structure only, so you still need to evaluate output quality. Repo is in maintenance mode.

## Recipe / links
- Repo: https://github.com/conorbronsdon/agent-skill-builder (MIT)
- Demo GIF in README shows valid skills passing and a broken one failing

## Why it made the cut
Small (~7★) but concrete, verifiable, and fills a gap next to SkillEvaluator / SkillSpector: authoring-time structural validation that can fail.
