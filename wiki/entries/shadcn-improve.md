# improve（shadcn，强模型审计 + 写计划，便宜模型执行）

**Tags:** code-audit, planning, refactor, multi-model, skill
**Source:** [@wy_ones](https://x.com/wy_ones/status/2120395449622503895) · 2026-11-11
**Engagement:** 帖子互动低 · shadcn/improve ~10k★ · MIT

## When to use
想用最强（最贵）的模型理解整个代码库、判断哪些改动值得做并写出规格，再把实现交给便宜模型或其他 agent；也适合 PR 前审当前分支、做安全/性能等专项审计、整理改进 backlog。

## What it does
`/improve` 先绘制仓库地图并审计，给出带优先级的发现表；你挑选后，它在 `plans/` 下为每项写一份自包含的实施计划（附推荐顺序）。技能本身不改代码。`/improve execute <plan>` 可在隔离 worktree 里派便宜模型执行并对照计划审 diff，合并仍由你决定；`/improve reconcile` 核对已落地、刷新漂移的计划。支持 quick / deep / security / branch / next / review-plan / `--issues` 等模式。

## Recipe / links
- Repo: https://github.com/shadcn/improve
- 安装：`npx skills add shadcn/improve`（Agent Skills 格式通用）
- 典型流程：`/improve` → 回复「plan 1, 3 and 5」→ 审阅 `plans/` → 交给执行 agent 或 `/improve execute 001` → 下次 `/improve reconcile`

## Why it made the cut
配方完整、命令清晰、产物是可审阅的纯 markdown 计划；作者知名、仓库社区信号强。「贵模型规划、便宜模型执行」的分工可直接复用。
