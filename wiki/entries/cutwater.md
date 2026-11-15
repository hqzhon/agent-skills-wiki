# CutWater（issue → PR 的 GitHub 工作流）

**Tags:** git, github, workflow, pr, skill
**Source:** [@YourAKShaw](https://x.com/YourAKShaw/status/2121595384103625202) · 2026-11-15
**Engagement:** 发现帖为作者说明帖（0 赞）；仓库 [YourAKShaw/CutWater](https://github.com/YourAKShaw/CutWater) v0.1.0，0★，Apache-2.0，带文档、evals 与 skills.sh 页面

## When to use
要让编码 agent 按 GitHub 原生流程干活：先审计/补齐仓库卫生，再把每件事做成 issue → 分支 → Conventional Commits → PR，由你审查并合并。不要用它来自动合入。

## What it does
每次调用先走 Phase 0（审计、询问、脚手架）：README、LICENSE、CONTRIBUTING、CODE_OF_CONDUCT、SECURITY、issue / PR 模板、CODEOWNERS、CI、Dependabot、labels、分支规则等。之后每个任务都走 issue → 分支 → 提交 → PR。硬性规则包括：永远不 `gh pr merge`、不启用 auto-merge、不把提交推到默认分支；破坏性操作和覆盖已有文件都要先给 diff、等你说 yes。需要已登录的 `gh`、git 和 Node 18+ 辅助脚本。

## Recipe / links
- Repo: https://github.com/YourAKShaw/CutWater（Apache-2.0，v0.1.0）
- Skill：https://github.com/YourAKShaw/CutWater/blob/main/skills/cutwater/SKILL.md
- 文档：https://github.com/YourAKShaw/CutWater/tree/main/docs
- 目录页：https://www.skills.sh/yourakshaw/cutwater/cutwater
- 安装（若用 skills CLI）：`npx skills add YourAKShaw/CutWater`
- 依赖：git、已认证的 GitHub CLI（`gh`）、Node.js 18+

## Why it made the cut
SKILL.md 把 GitHub 工作流写成可执行阶段和明确禁令（不合入、不覆盖不先问），仓库结构完整（文档、evals、插件清单）。星数为零、版本仍是 v0.1.0，但材料可验证，适合作为「agent 改代码也要留痕」的早期技能收录。
