# Humanizer-zh（中文去 AI 腔）

**Tags:** writing, chinese, anti-slop, editing, skill
**Source:** [@shshajs85](https://x.com/shshajs85/status/2114908190081192260) · 2026-10-27
**Engagement:** discovery post (low) · repo ~21.1K★

## When to use
When polishing **Chinese** articles, comments, or docs that read like industrial AI template prose — empty intensifiers, stock transitions, repetitive parallelisms — while keeping facts, certainty level, and the author’s voice.

## What it does
Claude/agent skill (`op7418/Humanizer-zh`) adapted from blader/humanizer. `SKILL.md` editing rules + examples: strip AI tells, don’t rewrite clean sentences, optional author samples for voice (without copying sample facts). Explicitly **not** an AIGC detector and does not claim to beat detectors.

## Recipe / links
- Repo: https://github.com/op7418/Humanizer-zh (~21.1K★)
- Install: `npx skills add https://github.com/op7418/Humanizer-zh.git`
- Alt: clone into `~/.claude/skills/humanizer-zh`
- Upstream EN inspiration: blader/humanizer (see also catalog [Stop Slop](stop-slop.md) for English anti-slop)

## Why it made the cut
Concrete Chinese SKILL.md with clear when-to-use boundaries, install recipe, and large community adoption — fills the ZH anti-slop gap next to Stop Slop.
