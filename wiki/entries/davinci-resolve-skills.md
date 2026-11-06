# DaVinci Resolve Skills（可继续剪的 Resolve 时间线）

**Tags:** video, davinci-resolve, remotion, tutorial, skill-pack
**Source:** [@Manojkumar2257](https://x.com/Manojkumar2257/status/2118547853694128628) · 2026-11-06
**Engagement:** 同帖 3 MIT skills；repo MusicProWorkshop/davinci-resolve-skills · MIT

## When to use
需要在 **DaVinci Resolve Studio** 里产出编辑器可继续改的时间线：截图教程走查、Remotion 视频迁入 Resolve、或 kinetic typography 片按节拍落 Fusion。不要用于只想要最终 mp4、不碰 Resolve 的流程。

## What it does
三个 skill（Claude plugin）：`resolve-screen-tutorial`（截图 + brief → 带缩放/光标/高亮/字幕的时间线）、`remotion-to-resolve`（从 Remotion 场景数据重建并 SSIM 对照）、`kinetic-film-to-resolve`（按拍点写 Fusion）。依赖 Resolve MCP `run_script_unsafe`；改完后由你自己保存工程。

## Recipe / links
- 仓库：https://github.com/MusicProWorkshop/davinci-resolve-skills
- 安装：`/plugin marketplace add MusicProWorkshop/davinci-resolve-skills` 后装 `davinci-resolve-timelines`
- SKILL 路径：`plugins/davinci-resolve-timelines/skills/*/SKILL.md`

## Why it made the cut
真实可执行配方 + 明确环境边界（Studio 21 + MCP）；开源 MIT。社区星数尚低，但步骤与限制写得很具体。
