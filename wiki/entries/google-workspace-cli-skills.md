# Google Workspace CLI Skills（gws）

**Tags:** skill-pack, gmail, calendar, drive, docs, cli, google-workspace
**Source:** [@xiaoanlab](https://x.com/xiaoanlab/status/2118332105184928034) · 2026-11-05
**Engagement:** discovery post; repo googleworkspace/cli ~32k★ · Apache-2.0

## When to use
要用 agent 批量处理 Gmail / Calendar / Drive / Docs / Sheets / Chat / Admin 等 Workspace 任务，又不想在网页来回切，或希望输出结构化 JSON 交给下游自动化时。

## What it does
`gws` 从 Google Discovery Service 动态生成命令；仓库 `skills/` 下带约 95 个 Agent Skills（如 `gws-gmail-triage`、`gws-calendar-agenda`、`gws-drive-upload`），每个 SKILL.md 声明前置二进制与安全规则，并指向共享 `gws-shared` 鉴权说明。非 Google 官方支持产品，仍在向 1.0 推进。

## Recipe / links
- Repo: https://github.com/googleworkspace/cli
- Skills 目录：https://github.com/googleworkspace/cli/tree/main/skills
- 示例 skill：`skills/gws-gmail-triage/SKILL.md` → `gws gmail +triage`
- 安装 CLI 后可用 `gws generate-skills` 刷新 skill 文件

## Why it made the cut
可执行 SKILL.md + 清晰 Workspace 场景；大仓库可核对；技能与 CLI 绑定，适合 agent 直接调。
