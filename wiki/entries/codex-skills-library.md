# Codex Skills Library

**Tags:** skill-pack, engineering, codex, devops, security, testing
**Source:** [@beebidao](https://x.com/beebidao/status/2117044560861990980) · 2026-11-02
**Engagement:** proflead/codex-skills-library ~167★（推文称 1,000+★，实测不符）

## When to use
想给 Codex（或任何读 `SKILL.md` 的 Agent）装一套小而专的日常工程技能：读陌生代码库、排错清单、解释报错、修 lint、审数据库迁移风险等，而不是每次重写提示词。

## What it does
按领域（foundation、api、architecture、backend、data、frontend、infra、performance、planning、reliability、security、testing、docs）组织的 skill 集合。每个 skill 是一个带 `name` / `description` frontmatter 的 `SKILL.md` 文件夹，流程短、可自然语言触发、按需加载。推文重点推荐的 `db-migration-reviewer` 用于在执行前审计 SQL 迁移的锁表、数据丢失等风险。

## Recipe / links
- Repo: https://github.com/proflead/codex-skills-library
- 例：`skills/foundation/codebase-orientation/SKILL.md`、`skills/foundation/debugging-checklist/SKILL.md`

## Why it made the cut
有成体系的 `SKILL.md` 仓库和清晰分域，单个 skill 粒度小、易挑选移植。社区热度不高（推文星数有夸大），按内容收录。
