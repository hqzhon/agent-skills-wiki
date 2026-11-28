# Eagerworks Skills（写 PR / 审查 / 交接等工程流程包）

**Tags:** git, pull-request, code-review, workflow, compliance, skill-pack
**Source:** [@eagerworks](https://x.com/eagerworks/status/2126300524303503489) · 2026-11-27
**Engagement:** 作者团队第一方介绍帖 7 赞，同串[回复给出仓库与安装命令](https://x.com/eagerworks/status/2126303274538254723)。仓库 [eagerworks/skills](https://github.com/eagerworks/skills) 现 18★，MIT。

## When to use
希望 coding agent 按团队真正在用的流程来写提交、开 PR、做代码审查、写架构决策或做仓库交接，而不是随口写一句 “fixed stuff” 就提 PR 时用。官方演示重点是 `create-pr`：它会写完整描述和测试计划，缺信息就问你，而不是编造。

## What it does
一套 10 个可单独安装的 Agent Skills，目前包括：
- Git 工作流：`commit`（按逻辑变更写 Conventional Commits，不 `git add -A`、不用 `--no-verify`）、`create-pr`、`pr-review`
- 工程与交付：`repo-handoff`、`decision-record`、`rest-api-design`、`mobile-store-review`、`kamal`
- 合规审计：`audit-hipaa`、`loop-engineering-audit`

适用于 Claude Code、Cursor、Copilot、Codex、Amp 等能读 Agent Skills 格式的工具。

## Recipe / links
- Repo: https://github.com/eagerworks/skills（18★，MIT）
- 先装演示里的 `create-pr`：
  ```bash
  npx skills add eagerworks/skills --skill create-pr
  ```
  或按需加上面列出的其他技能名。
- 仓库含 README 分技能说明、evals 与 changelog。

## Why it made the cut
第一方发布，配方具体（尤其是 PR 描述和测试计划不许编造），有可安装的 SKILL 目录和 MIT 许可。10 个技能是同一团队的日常流程，适合作为工程交付包收录。
