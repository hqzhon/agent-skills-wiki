# Main Session Orchestrator（单主会话编排多阶段项目）

**Tags:** orchestration, codex, ml-experiments, research, handoff, skill
**Source:** [@huanngzh](https://x.com/huanngzh/status/2117501904683151830) · 2026-11-03
**Engagement:** 仓库 huanngzh/oh-my-skills（新建，个位数★）；作者为 MV-Adapter（1.3k★）作者

## When to use
多阶段研究、模型训练实验（数据准备 → 训练 / 消融 → 评测报告）或较长的工程项目，想主要只和一个「Main」会话对话，由它拆阶段、派发执行会话、验收产物，并在跨会话时保住决策与进度。

## What it does
- Main 负责目标、计划、派发、验收和项目总览；执行会话只拿到有边界的阶段简报，交回可供下一阶段接续的产物。
- 以产物为准做验收（artifact-based acceptance），而不是听执行会话的口头汇报。
- 项目文件持久记录决策、负责人、输入、恢复命令和证据，支持断点续跑；附进度看板 / 经过核实的网页快照。
- 以 Agent Skills 格式编写，先面向 Codex；执行、委派、调度能力取决于宿主。

## Recipe / links
- Repo: https://github.com/huanngzh/oh-my-skills → `skills/main-session-orchestrator/SKILL.md`（连同 `references/`、`assets/`、`scripts/` 整个目录复制）
- 安装：复制到 `~/.agents/skills/`（团队仓库用 `.agents/skills/`），或直接让 Codex 从该仓库路径安装；新开会话后按名字调用

## Why it made the cut
上轮列入观察、本轮找到仓库：SKILL.md 有清晰的角色分工、验收和交接机制，适合长周期 ML 实验这类真实场景；可与 wiki 里的 autoresearch、ccpm 等编排类条目对照。社区信号尚弱。
