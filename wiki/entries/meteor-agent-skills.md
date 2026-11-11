# Meteor Agent Skills（官方，17 个 Meteor 3 技能）

**Tags:** meteor, javascript, official, skill-pack, migration
**Source:** [@meteorjs](https://x.com/meteorjs/status/2120194293113688567) · 2026-11-10
**Engagement:** meteor/agent-skills v1.1.0 · 官方维护（刚公开，星数尚少）

## When to use
用 Codex、Claude Code、Cursor 等 agent 开发、调试、迁移或部署 Meteor 3 应用时，尤其是从 Meteor 2 迁到 3、切到 Rspack 构建。

## What it does
17 个 skill：accounts、blaze、cli 安装、社区包、调试、部署、methods、现代构建栈、Mongo/Minimongo、native、pub/sub、React、安全、测试、TypeScript、`migrate-to-meteor-3`、`migrate-to-rspack`。v1.1.0 围绕官方 Meteor 3.6 整理，带验证交接文档。

## Recipe / links
- Repo: https://github.com/meteor/agent-skills
- 全量：`npx skills add meteor/agent-skills`（需 Node 22.20+）
- Claude Code：`claude plugin marketplace add meteor/agent-skills` → `claude plugin install meteor@meteor`；Codex：`codex plugin marketplace add meteor/agent-skills` → `codex plugin add meteor@meteor`

## Why it made the cut
框架官方出品，skill 按任务拆分且有版本化发布与迁移配方，是框架级技能包的规范样本。
