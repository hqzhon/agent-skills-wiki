# Jujutsu（jj）Agent Skill

**Tags:** vcs, jujutsu, git, agent-safety, skill
**Source:** [@404Cause](https://x.com/404Cause/status/2115203844363989221) · 2026-10-27
**Engagement:** author note · repo ~81★

## When to use
When the repo has a **`.jj/`** directory (or you use Jujutsu/jj) and an agent must do VCS work—raw `git` can corrupt jj state. Activate before commit/status/branch/push style operations, especially with detached HEAD.

## What it does
Teaches agents jj workflows for agent environments: always `--no-pager`, inline `-m` messages (no editors), verify with `jj st` after mutations, working-copy-as-commit model, squash/split without a staging area. Tested against jj v0.37.0.

## Recipe / links
- Repo: https://github.com/danverbraganza/jujutsu-skill (~81★)
- Skill: `jujutsu/SKILL.md` (install via `just install` or copy into `.claude/skills/`)
- Related: netresearch/jujutsu-workflow-skill and other jj skills exist; this is the author’s starred personal skill

## Why it made the cut
Concrete agent-safety recipe for a real VCS footgun, installable SKILL.md, and clear when-to-activate gate.
