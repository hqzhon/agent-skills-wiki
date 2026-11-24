# PM Skills（产品决策框架市场，72 个技能 / 9 个插件）

**Tags:** product, pm, strategy, discovery, prioritization, skill-pack
**Source:** [@PawelHuryn](https://x.com/PawelHuryn/status/2124984448106009025) · 2026-11-24
**Engagement:** 本窗作者介绍帖 13 赞 / 17 收藏 · 仓库 [phuryn/pm-skills](https://github.com/phuryn/pm-skills) 现 28,260★，MIT · 与已收录的 [product-engineering](product-engineering.md) 是同一作者的配套仓库

## When to use
做产品决策（发现、策略、优先级、PRD、发布、增长），希望 agent 按 Teresa Torres / Marty Cagan 等既有框架走，而不是只生成更快的空文档。新想法可走 `/discover`，要战略清晰度走 `/strategy`，写 PRD 走 `/write-prd`。

## What it does
72 个 PM 技能和 42 条串联工作流，分成 9 个插件：`pm-toolkit`、`pm-product-strategy`、`pm-product-discovery`、`pm-market-research`、`pm-data-analytics`、`pm-marketing-growth`、`pm-go-to-market`、`pm-execution`，以及工具箱里的优先级框架等可单独引用的技能（本窗介绍的就是其中的 9 套优先级框架）。技能会在相关对话里自动加载；命令完成后再提示下一步。

作者把 AI 写代码、测试与发布门禁放在配套仓库 `phuryn/product-engineering`（本目录已收录为 [product-engineering](product-engineering.md)），本包专注产品决策本身。

## Recipe / links
- Repo: https://github.com/phuryn/pm-skills（28,260★，MIT）
- Claude Cowork：Customize → Browse plugins → Personal → 从 GitHub 添加市场 `phuryn/pm-skills`（9 个插件一次装齐）
- Claude Code：
  ```bash
  claude plugin marketplace add phuryn/pm-skills
  claude plugin install pm-toolkit@pm-skills
  claude plugin install pm-product-strategy@pm-skills
  claude plugin install pm-product-discovery@pm-skills
  claude plugin install pm-market-research@pm-skills
  claude plugin install pm-data-analytics@pm-skills
  claude plugin install pm-marketing-growth@pm-skills
  claude plugin install pm-go-to-market@pm-skills
  claude plugin install pm-execution@pm-skills
  ```
- AI Shipping 插件已迁到配套仓：`claude plugin install ai-shipping@product-engineering`

## Why it made the cut
同一作者已收录的 product-engineering 是「把产品做出来」的工程技能包（608★）；本仓库是 28k★ 的产品决策框架市场，有明确命令、9 个插件和可验证的 `SKILL.md`。本窗由作者本人介绍优先级框架，按高星漏收补上，两套应一起看、不要当成重复条目。
