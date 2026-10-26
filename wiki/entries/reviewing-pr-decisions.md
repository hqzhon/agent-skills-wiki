# reviewing-pr-decisions（Nishant PR review skill）

**Tags:** code-review, pull-request, claude-code, skill
**Source:** [@n1sh4n7](https://x.com/n1sh4n7/status/2114650366897967329) · 2026-10-26
**Engagement:** discovery post (low); companion essay + example HTML review page

## When to use
When coding agents flood PRs with noisy diffs and you want a review page of the *judgment calls* (before/after pairs + one question each) instead of reading every file—without the skill telling you to merge.

## What it does
Claude/agent skill that builds an HTML review of PR decisions, plus a second independent pass for security/performance that never sees the first review. Needs GitHub CLI (`gh`) logged in. Example output included in-repo.

## Recipe / links
- Repo: https://github.com/nishantc7/skills
- Skill folder: `reviewing-pr-decisions/` (copy into `~/.claude/skills/`)
- Essay: https://nishantc7.github.io/writing/2026/10/25/code-review-after-coding-agents/
- Example: https://raw.githack.com/nishantc7/skills/main/reviewing-pr-decisions/example-review.html

## Why it made the cut
Concrete SKILL.md + install steps; clear post-agent code-review use case; verifiable repo, essay, and sample HTML (not vaporware).
