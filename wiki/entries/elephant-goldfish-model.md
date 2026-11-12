# Elephant-Goldfish Model（Google，带上下文起草 + 无记忆评审）

**Tags:** design-review, spec, planning, subagents, official, plugin
**Source:** [@buzhimingyanyua](https://x.com/buzhimingyanyua/status/2120742552274100679) · 2026-11-12
**Engagement:** 帖子互动低 · google/elephant-goldfish-model ~17.7k★

## When to use
动手实现前要把一个需要设计决策的功能写成规格，并想让「没看过之前对话」的评审者挑出隐含假设和盲点；也适合拿现有设计文档 / README / PR 计划对照真实代码做评审，或检查文档与代码是否已漂移。

## What it does
Elephant（持有项目上下文的主会话）和你一起头脑风暴、起草 `design_draft.md`，每节暂停等你反馈；Goldfish（全新、只读的子 agent 评审者）只看草稿和引用的源码，从设计、清晰度、与代码契合度、实施计划几个角度出意见。由你取舍发现、批准规格后再实现。另有 `egm-drift-report` 比对文档与当前代码，`egm-review-loop` 可自选评审者与标准审其他类型文档。

## Recipe / links
- Repo: https://github.com/google/elephant-goldfish-model · 官网 https://egm.dev
- Claude Code：`claude plugin marketplace add google/elephant-goldfish-model` → `claude plugin install egm@egm`
- Codex CLI：`codex plugin marketplace add google/elephant-goldfish-model` → `codex plugin add egm@egm`；Antigravity：`agy plugin install https://github.com/google/elephant-goldfish-model`
- 流程：`/egm:egm-brainstorm <需求>` → `/egm:egm-draft` → `/egm:egm-review design_draft.md`；60 秒试用：`/egm:egm-review docs/designs/x.md`、`/egm:egm-drift-report docs/designs/`
- 注意：要装完整插件，只拷 `skills/` 不够（运行时还要读 `agents/` 和 `resources/document_standards/`）；需要能起全新子 agent 的会话

## Why it made the cut
Google 官方开源、配方完整、命令清晰；「有上下文的人起草、无上下文的人评审」是可直接复用的设计评审模式，社区信号强。
