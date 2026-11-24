# scenario-selfie-hologram（自拍登记成会说话的 3D 全息影像）

**Tags:** video, 3d, hologram, scenario, skill
**Source:** [@AIandDesign](https://x.com/AIandDesign/status/2124950659342750117) · 2026-11-23
**Engagement:** 本窗作者介绍帖 3 赞 / 1 收藏 · 仓库 [TheMarco/Scenario-Selfie-Hologram](https://github.com/TheMarco/Scenario-Selfie-Hologram) 现 0★，MIT，含 `SKILL.md`、本地 HoloMe CLI 与演示视频

## When to use
想从几张自拍登记一个人，再把手机自拍视频变成会跟着真实口型、眨眼和头部动作说话的全息影像（带自己的声音）；输出可合成的 ProRes 4444（带 alpha 的 `.mov`）和黑底 H.264 `.mp4`。

## What it does
Claude Code 技能：登记阶段把 1–5 张自拍（或从自拍视频抽帧）交给 Scenario MCP，用 GPT Image 做三视图角色表、用 Tripo 出 3D 头，再在本地用捆绑的 HoloMe CLI 绑定和渲染。登记每人约 255 Scenario CU。本地 `setup.sh` 会装约 1.6 GB（Python 3.12 venv、Node 包、MediaPipe、渲染器、Depth Anything 与 Whisper 权重）。后续同一人的视频只驱动动作，不再重新登记。

依赖第三方 Scenario 账户与 MCP，以及较大的本机模型权重，不是纯离线技能。

## Recipe / links
- Repo: https://github.com/TheMarco/Scenario-Selfie-Hologram（0★，MIT）
- 安装：
  ```bash
  git clone https://github.com/TheMarco/Scenario-Selfie-Hologram.git ~/.claude/skills/scenario-selfie-hologram
  ~/.claude/skills/scenario-selfie-hologram/tool/setup.sh
  claude mcp add --transport http --scope user scenario https://mcp.scenario.com/mcp
  ```
  然后在 Claude Code 里 `/mcp` 登录 Scenario。可用 `--no-prefetch` 把模型权重留到首次使用再下载。
- 用法：`/scenario-selfie-hologram`，或「用这些自拍登记我为全息影像」「把这段自拍视频做成竖屏全息」。

## Why it made the cut
有完整 `SKILL.md`、本机渲染 CLI、演示和明确的输入/输出格式。星数为 0 且依赖付费 Scenario 额度，但配方可执行，不是一句「做成全息」的空话。收录时标明云端费用和 1.6 GB 本地安装。
