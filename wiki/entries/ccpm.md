# CCPM（Project Manager Agent Skill）

**Tags:** project-management, prd, github-issues, parallel-agents, skill-pack
**Source:** [@perry_weijie](https://x.com/perry_weijie/status/2116016132234613217) · 2026-10-30
**Engagement:** tip post; material = automazeio/ccpm ~8423★ MIT

## When to use
When you want an agent to act as a **产品经理脑**：点子 → 可评审 PRD → Epic → GitHub Issues → 多 agent 并行写代码，全程可追溯，而不是在聊天里丢上下文。

## What it does
CCPM（Claude / Agent Code Project Manager）是标准 Agent Skill：用 GitHub Issues + git worktrees 组织并行执行。口述需求可引导出 PRD，Epic 拆成带依赖的并行任务，再落到 Issues 与生产代码。需要 `git` + 已登录的 `gh`，以及项目对应的 GitHub 仓库。

## Recipe / links
- Repo: https://github.com/automazeio/ccpm
- Skill path: `skill/ccpm/`（含 `SKILL.md` + `references/`）
- Install（示例）:
  - `git clone https://github.com/automazeio/ccpm.git`
  - Claude Code: `ln -s /path/to/ccpm/skill/ccpm .claude/skills/ccpm`
  - 其他兼容 harness：指向 `skill/ccpm/`
- Prerequisites: `gh auth login`

## Why it made the cut
High-star MIT pack with a concrete PRD→Issues→parallel-agents recipe and an agentskills.io-compatible folder—fills the “PM for coding agents” gap beyond tipster listicles.
