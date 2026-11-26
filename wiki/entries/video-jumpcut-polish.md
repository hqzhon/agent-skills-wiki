# video-jumpcut-polish（macOS：口播/开箱毛片一键精剪）

**Tags:** video, jumpcut, macos, ffmpeg, subtitles, skill
**Source:** [@zhanghe](https://x.com/zhanghe/status/2125809883467682269) · 2026-11-26
**Engagement:** 作者开源帖 1 赞；仓库 [zh30/video-jumpcut-polish](https://github.com/zh30/video-jumpcut-polish) 现 0★，MIT，2026-11-26 新建并推送。

## When to use
在 **macOS 14+**（推荐 Apple Silicon）上，把口播、播客片段或开箱毛片自动剪成可发布成片时用：去掉死气和口头禅、降环境混响、修 iPhone HDR、模糊隐私屏幕、做不乱改五官/产品的封面，并写出适合 5 个平台的标题和 SEO 文案。需要本机 `ffmpeg`。不要在 Linux / Windows 上指望同一条流水线，也不是通用时间线剪辑器（那类更接近 [video-use](video-use.md)）。

## What it does
把编码 agent 变成本机后期工作室：Python 标准库 + 自动编译的 Swift 助手，调用 Apple Neural Engine 人声隔离（`AUSoundIsolation`）、Vision、CoreText、VideoToolbox，**零 pip 依赖**。README 强调关键帧概览、自动补偿人声隔离的 76.4 ms 前瞻延迟（宣称 0.0 ms A/V 不同步），以及按体裁调整的流水线和五平台发布文案。技能文件在 `skills/video-jumpcut-polish/SKILL.md`。

## Recipe / links
- Repo: https://github.com/zh30/video-jumpcut-polish（0★，MIT）
- 安装：`npx skills add zh30/video-jumpcut-polish`（Antigravity / Claude Code / Cursor / Codex）
- 技能：[skills/video-jumpcut-polish/SKILL.md](https://github.com/zh30/video-jumpcut-polish/blob/main/skills/video-jumpcut-polish/SKILL.md)
- 前置：macOS 14+、`ffmpeg`；推荐 Apple Silicon

## Why it made the cut
本窗作者刚发布的完整可加载技能，平台限制和依赖写得很清楚。仓库尚无 star，按完整配方收录，不是凭热度。未在本机实测，以 README 为准。
