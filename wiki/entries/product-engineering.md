# Product Engineering（从想法到上线的 45 个技能包）

**Tags:** product, engineering, skill-pack, shipping, claude-code
**Source:** [@PawelHuryn](https://x.com/PawelHuryn/status/2122017820657455466) · 2026-11-16
**Engagement:** 原帖互动很少 · 仓库 [phuryn/product-engineering](https://github.com/phuryn/product-engineering) 现 608★ / 81 forks，MIT · 作者 @PawelHuryn（The Product Compass）

## When to use
产品经理、创始人或工程师用 Claude Code、Codex、Cursor 等编码助手，从「决定做什么」做到上线、收款和多人协作评审，而不只是写代码。不确定当前该用哪一条时，可先走 `/product:start-here`（Codex 为 `$product:start-here`）。

## What it does
45 个可加载 `SKILL.md`，分成 6 个插件包，来自作者已经上线的三款产品（AskOne、Staygreen、AFK Pilot）的实操经验：

- **product**：选题、细分市场、价值主张、竞品与增长，以及 `start-here` 路由
- **ai-shipping**：代码评审、独立模型复核、测试与发布门禁、安全/性能静态检查
- **agent-teams**：在 Claude / Codex / Gemini / Grok 之间委派
- **agent-harness**：说明文件、交接、回顾、护栏 hooks
- **app-stack**：UI、鉴权、MCP、分析、监控、法律页等上线栈
- **work-humanizer**：把产出改得不像机器腔

技能可用于 Claude Code、Codex、Cursor、Gemini CLI、OpenCode、GitHub Copilot 等能读取 `SKILL.md` 目录的环境。

## Recipe / links
- Repo: https://github.com/phuryn/product-engineering（608★，MIT）
- 介绍文：https://www.productcompass.pm/p/product-engineering-skills
- 案例：仓库内 [CASE-STUDIES.md](https://github.com/phuryn/product-engineering/blob/main/CASE-STUDIES.md)
- 最快安装：在项目目录里让 agent 执行「Please install skills from phuryn/product-engineering on GitHub in this project only. Enable auto updates.」
- Claude Code 插件市场：
  ```bash
  claude plugin marketplace add phuryn/product-engineering
  claude plugin install product@product-engineering
  claude plugin install ai-shipping@product-engineering
  claude plugin install agent-teams@product-engineering
  claude plugin install agent-harness@product-engineering
  claude plugin install app-stack@product-engineering
  claude plugin install work-humanizer@product-engineering
  ```
  可加 `--scope project` 或 `--scope local`。装完后开启该 marketplace 的自动更新，再运行 `/product:start-here`。

## Why it made the cut
有完整仓库、MIT 许可、明确安装路径和 45 条可核验技能，并且用三款已上线产品做案例，而不是空清单。社区信号来自仓库本身（608★），不只看原帖互动。
