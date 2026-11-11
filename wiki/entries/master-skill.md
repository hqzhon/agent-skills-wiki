# 大师.skill（把整个行业蒸馏成 skill）

**Tags:** skill-authoring, research, industry, distillation, chinese, skill
**Source:** [@Blackmambaer](https://x.com/Blackmambaer/status/2120390876778361076) · 2026-11-11
**Engagement:** 帖子互动低 · swaylq/master-skill ~180★ · MIT

## When to use
想让 agent 进入某个细分行业「资深从业者」模式：先自动调研该行业的头部人物、工具、工作流、知识经典、信息源和术语，再生成一个可装载的行业 skill 加配套命令行工具。

## What it does
输入行业名后，按 6 条线（行业大佬 / 工具地图 / 工作流 / 知识正典 / 信息源 / 术语标准）自动调研，约 30–60 分钟蒸馏出「行业 Master OS」SKILL 和一套 bash 命令。产物可装到 Claude Code、Codex、OpenClaw 等 agent。是「同事.skill」「女娲.skill」一类蒸馏技能的行业版。

## Recipe / links
- Repo: https://github.com/swaylq/master-skill （Python + Shell，带 CI）
- 官网: https://master-skill.org/
- 兼容 skills.sh 安装

## Why it made the cut
有完整生成流程和仓库、场景清晰，是「生成 skill 的 skill」中较具体的一个。社区信号较弱，产物质量取决于调研来源，使用前应人工审阅生成的 SKILL.md。
