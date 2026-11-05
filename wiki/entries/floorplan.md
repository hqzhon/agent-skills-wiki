# Floorplan（代码库大白话交互地图）

**Tags:** codebase, architecture, visualization, onboarding, claude-code, codex
**Source:** [@Lingze688](https://x.com/Lingze688/status/2118217123285852414) · 2026-11-05
**Engagement:** 仓库 haydenschmitty/floorplan，约 2.9k★，MIT，2026-10-27 创建

## When to use
接手陌生项目、给非技术同事讲清楚系统怎么拼起来、或者多仓库应用想要一张「谁调用谁」的全景图时。

## What it does
让 Claude Code 或 Codex 读代码库，画出一张可交互的地图：每个模块、文件和 Web 请求都配一个大白话名字，模块之间的连接全部画出来。以 Claude Code / Codex 插件形式分发，Node 18+、零依赖，有在线 demo（一个跨四个仓库的咖啡订阅示例应用）。

## Recipe / links
- Repo: https://github.com/haydenschmitty/floorplan
- 在线 demo: https://haydenschmitty.github.io/floorplan-demo/
- 仓库内 `skills/` 目录 + `.claude-plugin` / `.codex-plugin` 插件清单，README 有与 archify 等同类工具的对比

## Why it made the cut
有完整仓库、测试和 demo，场景清晰；与已收录的 stack-diagram（按描述画架构图）互补，这个是从真实代码反推结构。
