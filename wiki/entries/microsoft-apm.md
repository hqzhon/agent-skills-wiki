# APM — Agent Package Manager（Microsoft）

**Tags:** package-manager, skill-infra, install-hygiene, lockfile, multi-agent, microsoft
**Source:** [@hsianghui](https://x.com/hsianghui/status/2120904514546843714) · 2026-11-12
**Engagement:** 原帖热度低；仓库 microsoft/apm ~4.3k★ · Apache-2.0

## When to use
团队在多个 agent（Copilot、Claude Code、Cursor、Codex、Gemini、OpenCode 等）间共享技能、提示词、hooks 和 MCP 服务器，希望「克隆仓库 → 一条命令装好全部 agent 配置」，并且能锁版本、可复现、可审计。

## What it does
- 在项目里的 `apm.yml` 声明依赖：任意仓库里的单个技能（如 `anthropics/skills/skills/frontend-design`）、插件、agent 文件、完整 APM 包和 MCP 服务器
- `apm install` 解析传递依赖并部署到所选 agent；`apm.lock.yaml` 锁定解析结果与内容哈希
- 兼容 `npx skills add` 的用法：`apm install vercel-labs/agent-skills --skill deploy-to-vercel`，同时写入清单
- `apm audit` 扫描隐藏 Unicode 等可疑内容；支持 marketplace、打包（`apm pack`）、导出 `plugin.json`，以及 GitHub Action

## Recipe / links
- 仓库：https://github.com/microsoft/apm · 文档 / Quick Start：https://microsoft.github.io/apm/quickstart/
- 最小流程：在项目根写 `apm.yml`（targets + dependencies）→ `apm install` → 把 `apm.yml` 和 `apm.lock.yaml` 一起提交

## Why it made the cut
配方具体、场景清楚、仓库可核且有一定星数；它解决的是技能「怎么可复现地装、怎么锁版本」，可与 [SkillSpector](skillspector.md)（装前安全扫描）、[SkillHub](iflytek-skillhub.md)（企业注册中心）搭配。
