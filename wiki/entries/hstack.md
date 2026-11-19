# hstack（大模型编排小模型并行交付）

**Tags:** orchestration, cost, multi-agent, worktree, skill-pack
**Source:** [@shellhaki](https://x.com/shellhaki/status/2123189263248359441) · 2026-11-19
**Engagement:** 作者本人介绍帖（约 1 赞）；仓库 [shellhaki/hstack](https://github.com/shellhaki/hstack) 为 2026-11-18 新建、0★，MIT（早期条目）。作者称灵感来自 poteto 的 pstack，但实现不同。

## When to use
任务够大（大约 500+ 行新代码或 10+ 个文件）、能拆成 2–6 个文件互不重叠的工作包、且每个包都有机械检查（类型 / lint / 测试）时，让前沿模型当技术负责人，把大量写代码的工作交给更便宜的小模型并行完成。不适合小改动或强耦合改动。

## What it does
一套技能：`hstack`（入口与编排）、`hstack-plan`（写规格、冻结契约、按工人拆任务书）、`hstack-run`、`hstack-verify`。大模型先写规格、再在隔离 git worktree 里并行拉起工人（默认 Muse Code，也可用其他 CLI agent），等待而不轮询，对照测试和真实服务验收后再合并。仓库还带 `scripts/`（setup / run / progress / collect / merge / cleanup）和 `templates/`、`benchmarks/`。

## Recipe / links
- Repo: https://github.com/shellhaki/hstack（MIT，0★）
- 安装：
  ```bash
  git clone https://github.com/shellhaki/hstack ~/hstack
  cd ~/hstack
  ./install.sh claude     # 或 codex / muse / 任意 skills 目录
  ```
  安装为软链，`git -C ~/hstack pull` 即可更新。
- 依赖：`git`、`bash`，以及工人 CLI 在 `PATH` 上（默认 `muse`）；可选 macOS Terminal 或 tmux 看各工人窗口。

## Why it made the cut
不是「再包一层路由」，而是把计划、并行工单、worktree 隔离和验收写成可加载技能与脚本；有明确的委派门槛。仓很新、星数为零，属早期收录。
