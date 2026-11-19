# lemo-animi（一句话做定格动画短片）

**Tags:** video, stop-motion, animation, codex, skill
**Source:** [@ai_bange](https://x.com/ai_bange/status/2123319390255112685) · 2026-11-19（转述官方 [@lemomo_ai](https://x.com/lemomo_ai/status/2123038832815907084)）
**Engagement:** 转述帖约 8 赞级互动；仓库 [lemomo-ai/lemo-animi](https://github.com/lemomo-ai/lemo-animi) 100★。许可证为 CC BY-NC 4.0（非商业免费，商用需另谈授权）。

## When to use
想用 **Codex 或 Claude Code**，用一句话做成一支**定格动画短片**（黏土、纸艺、铁皮玩具等固定材质），并且希望「生图负责像、代码负责动」、而不是走视频生成模型时使用。

## What it does
Agent 先写故事和镜头表，按八种材质包出角色设定、八格动作表和背景，抠图后在代码里逐帧摆拍；再用真实乐器采样配乐、加拟音，打开审片台，你写意见它改，直到通过。八种风格（clay / papercraft / tin / felt / cardboard 等）各有提示词、灯光、镜头语法和拟音包，仓库带样片与画廊。Claude Code 可跑流程，画图默认交给本机 Codex 生图（或自备适配脚本）。首次运行会在 `~/lemo-animi-env` 准备 Python 环境和约 1.4 GB 采样库。

## Recipe / links
- Repo: https://github.com/lemomo-ai/lemo-animi（CC BY-NC 4.0，100★）
- 画廊：https://lemomo-ai.github.io/lemo-animi/ · [中文 README](https://github.com/lemomo-ai/lemo-animi/blob/main/README.zh-CN.md)
- Codex：
  ```
  codex plugin marketplace add lemomo-ai/lemo-animi
  codex plugin add lemo-animi@lemomo-ai
  ```
- Claude Code：`/plugin install lemo-animi --marketplace lemomo-ai/lemo-animi`，然后 `/reload-plugins`。成片命令很多，建议开 auto mode。
- 也可 clone 后把 `plugin/skills/lemo-animi` 链到 `~/.agents/skills` 或 `~/.claude/skills`。
- 依赖：macOS 或 Linux、ffmpeg、Python 3.11–3.13（或 uv）。
- 用法：「做一支 40 秒的黏土定格动画：小企鹅学做煎饼。」

## Why it made the cut
和已收录的 lemo-opuscar（影片风格工具箱）不是同一件事：这是可安装的定格短片配方，带 SKILL.md、材质包、审片流程和可下载样片。需注意非商业许可，以及生图依赖。
