# video-use（对话式剪辑 · browser-use）

**Tags:** video, editing, ffmpeg, talking-head, subtitles, skill
**Source:** [@Manojkumar2257](https://x.com/Manojkumar2257/status/2118564056970010627) · 2026-11-06
**Engagement:** browser-use/video-use · ~30k★ · MIT

## When to use
把一文件夹口播 / 教程 / 旅行 / 采访毛片交给 coding agent，用对话剪成 `final.mp4`：去 filler、调色、烧字幕、叠动画。不要用于「只生成画面、不剪真实素材」的纯文生视频。

## What it does
根目录超长 `SKILL.md` + `helpers/`：词级转写 → 确认策略 → 分段无损拼接 → 30ms 音频淡入淡出 → 字幕最后烧录等硬规则；可并行子 agent 生成 HyperFrames / Remotion / Manim / PIL 叠加。会话记忆写在素材旁 `edit/project.md`。

## Recipe / links
- 仓库：https://github.com/browser-use/video-use
- SKILL.md：https://github.com/browser-use/video-use/blob/main/SKILL.md
- 安装说明：https://github.com/browser-use/video-use/blob/main/install.md
- 另有 `skills/manim-video/SKILL.md`

## Why it made the cut
超强社区信号 + 生产向硬规则写死；可验证材料完整；MIT。
