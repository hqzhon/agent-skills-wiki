# EvoSkill（从失败轨迹自动生成 / 改进 skill）

**Tags:** meta, skill-generation, evaluation, self-improvement, claude-code, codex
**Source:** [@zyvre_ic](https://x.com/zyvre_ic/status/2117678291754615110) · 2026-11-04
**Engagement:** 仓库 sentient-agi/EvoSkill 约 1.3k★（Apache-2.0），附论文与官方博客

## When to use
你有一个可打分的任务集（基准、内部 eval），agent 总在某类任务上失败，想让它从失败里归纳出可复用的 skill / prompt，而不是直接换更大的模型。

## What it does
- 读取 agent 的失败轨迹，联合提出多个 skill 与 prompt 变体，在留出数据上评估，每轮产出一个新的 agent 程序（把 GEPA 的单文件优化扩展到整个 agent）。
- 支持 Claude Code、Codex CLI、OpenCode、OpenHands、Goose、Harbor 等，模型提供方可自选。
- 作者报告在电子表格任务上 40.4% vs 32.7%（来自推文 / 项目材料，未独立验证）。

## Recipe / links
- Repo: https://github.com/sentient-agi/EvoSkill
- Paper: https://www.alphaxiv.org/abs/2603.02766
- Blog: https://www.sentient.xyz/blog/evoskill-automated-skill-induction-from-agent-failures
- 用法：安装后 `evoskill init` 配好 agent 与基准，再 `evoskill run` 迭代

## Why it made the cut
不是单个 skill，而是「把失败变成 skill」的生成与评估工具，有仓库、论文和清晰的使用前提（需要可打分的任务集）。与 SkillOpt、SkillSpector 同属 skill 工程类工具。
