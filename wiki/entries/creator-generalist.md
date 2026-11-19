# creator-generalist（2D/3D 社媒内容技能包）

**Tags:** video, 3d, 2d, social, blender, skill-pack
**Source:** [@dextune](https://x.com/dextune/status/2123249654208839867) · 2026-11-19
**Engagement:** 介绍帖约 8 赞 / 2 转发 / 7 书签；仓库 [codepawl/creator-generalist](https://github.com/codepawl/creator-generalist) 310★，MIT。

## When to use
要让 agent 做 YouTube / TikTok / Instagram / X 等平台的 2D 解说图、3D Short、过场或小型游戏内容，并希望先出廉价预览再渲最终成片时使用。不适合「一句提示直接出片、不要确认」的流程。

## What it does
一套可加载技能包。三条主技能 `3d-generalist`、`2d-generalist`、`game-generalist` 负责整条成片，再调用建模、绑定、动画、剪辑、声音等工艺技能。用户不必点名技能：直接说要做什么，或用 `/3dg`、`/2dg`、`/gameg`。动手前会就目的、平台、格式、风格逐项提问（每项带建议答案），先做廉价预览，再走 QA 门。3D 路径可用 Blender、Three.js 或作者的 Crucible，素材强调 CC0 / CC BY 扫描件。另有 `watch-video`、`design-sound` 插件。

## Recipe / links
- Repo: https://github.com/codepawl/creator-generalist（MIT，310★）
- 其他 agent（推荐）：
  ```bash
  npx skills add codepawl/creator-generalist
  ```
- Claude Code：
  ```bash
  claude plugin marketplace add codepawl/creator-generalist
  claude plugin install 3d-generalist@creator-generalist
  claude plugin install 2d-generalist@creator-generalist
  claude plugin install game-generalist@creator-generalist
  claude plugin install watch-video@creator-generalist
  claude plugin install design-sound@creator-generalist
  ```
- 常见依赖（按 README / INSTALL.md）：Blender 4.2+、FFmpeg、Node 20+、Python 3.10+；装前让 agent 按 `INSTALL.md` 检查本机工具，系统级安装需先问用户。

## Why it made the cut
不是再发一套空提示词，而是把提问、预览、QA 和 2D/3D/游戏三条主路径写成可安装技能包，安装说明按宿主拆开。与已有 Blender Agent Skills、Open 3D Skills 互补：这边偏社媒成片工作流。
