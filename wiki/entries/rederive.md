# rederive（苏格拉底式重推设计）

**Tags:** education, socratic, codebase, learning, skill
**Source:** [@vintcessun](https://x.com/vintcessun/status/2121869821575078201) · 2026-11-15
**Engagement:** 13 likes / 1 repost / 18 replies · [EricJujianZou/rederive](https://github.com/EricJujianZou/rederive) 现 838★，MIT

## When to use
想真正搞懂一个代码库（自己的仓库、本地路径或任意开源仓库的 git URL），而不是让 agent 把设计直接讲给你听：例如要向别人讲解自己用 AI 写的项目、准备面试，或学习一个知名开源项目是怎么长出来的。

## What it does
可安装的 coding agent skill。它先在后台阅读代码、依赖和设计变更，把仓库拆成 5～10 个问题；前台不直接给答案，而是从「根问题」出发逐步加约束，让你自己推出方案。状态写在仓库的 `.rederive/`（加入 `.git/info/exclude`），不会去跑该仓库自己的脚本、安装步骤或测试。仓库里的文档和注释只当教材，不当指令。

## Recipe / links
- Repo: https://github.com/EricJujianZou/rederive（838★，MIT）
- 安装：`npx skills add EricJujianZou/rederive`（也可加 `-g` 装到本机所有项目）
- Claude Code 插件：`/plugin marketplace add EricJujianZou/rederive`，再 `/plugin install rederive@rederive`
- Skill 正文：仓库 `skills/rederive/SKILL.md`
- 依赖：`git`、`bash`、`python3`；在 agent 里输入 `/rederive`

## Why it made the cut
完整 SKILL.md、安装命令清楚，苏格拉底流程和安全边界写得很硬（不执行目标仓代码）。838★、MIT，和 Jane Street 的 socratic-tutor 互补：一个教主题，一个教代码库设计。
