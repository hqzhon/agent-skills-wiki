# Reelsmith Media（素材文件夹 → Instagram 竖版 Reel）

**Tags:** video, reels, captions, whisper, ffmpeg, skill
**Source:** [@Manojkumar2257](https://x.com/Manojkumar2257/status/2116494847658037521) · 2026-10-31
**Engagement:** tipster; material = EmirhanYAZICI/reelsmith-media（新仓库，星少）MIT, CI green

## When to use
你已经有配音、分镜片段、脚本和 logo，想要稳定、品牌一致的 1080×1920 竖版 Reel，而不想手工对字幕、调节奏、混音和导出。

## What it does
放一个文件夹：`voiceover.mp3`、`scene1.mp4…`、`script.txt`、`logo.png`，然后 `/reelsmith-media my-brand`。本地 Whisper 转写配音，再按脚本拼写校正字幕（品牌名不出错）；把每段片段慢放到对齐旁白（帧插值 + 裁切运镜）；加移动 logo 水印、转场；音频 -14 LUFS、语音时压低片段原声；30fps H.264 导出。前后各有检查：开工前查缺文件 / 坏文件，完成后核对尺寸、帧率、响度和画面冻结。全部本地运行，无付费 API。

## Recipe / links
- Repo: https://github.com/EmirhanYAZICI/reelsmith-media
- `npx skills add EmirhanYAZICI/reelsmith-media`（同时装 `reelsmith-media` 和 `whisper-tr`）
- 仍需本机有 ffmpeg、Python 3.10–3.12 + faster-whisper、HyperFrames、OpenMontage；README 有一键安装脚本
- 支持 Claude Code / Cursor / Codex / OpenCode / Antigravity

## Why it made the cut
配方非常具体（输入约定、固定步骤、前后检查、量化输出），仓库 + CI + demo 可验证；社区信号还弱，但材料扎实。
