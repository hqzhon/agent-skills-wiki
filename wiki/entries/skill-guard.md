# skill-guard

**Tags:** security, install-hygiene, trust-gate, claude-code
**Source:** [@nokslabs](https://x.com/nokslabs/status/2114698364361359484) · 2026-10-26
**Engagement:** launch post (low) · open CLI trust gate for skills

## When to use
When you want skills to load **only after a human approved that exact content**—and to block silent updates—via Claude Code / Pi hooks, complementary to vulnerability scanners like SkillSpector.

## What it does
CLI trust gate: deterministic content hash over a skill directory, rule-based scan with severities, approve/accept/block registry (`.agents/skills-trust.json`), and PreToolUse / UserPromptSubmit gates so unapproved, changed, or blocked skills never reach the model.

## Recipe / links
- Repo: https://github.com/NoksLabs/skill-guard
- Install: `npm install -g skill-guard` (Node ≥22.18)
- Commands: `skill-guard scan|approve|accept|block|setup`

## Why it made the cut
Clear supply-chain use case + concrete CLI recipe and gate hooks; verifiable public repo (complements SkillSpector rather than duplicating CVE scanning).
