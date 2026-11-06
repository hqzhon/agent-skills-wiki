# ai-video-skills（视觉圣经 + 打斗物理编排）

**Tags:** video, short-drama, consistency, choreography, skill-pack, chinese
**Source:** [@calmrisewild](https://x.com/calmrisewild/status/2118517276542669130) · 2026-11-06
**Engagement:** 作者自述数千镜头返工沉淀；repo xuyewild/ai-video-skills · MIT · 中英双语

## When to use
AI 漫剧 / 短剧 / 动画短片要跨集锁定画风比例，或把「激烈交锋」写成可生成的 setup→contact→result 节拍时。单条试玩短视频用不上。

## What it does
两个可分装 skill（`skills/en/` 与 `skills/zh/` 内容对等）：
- **visual-bible**：一两屏锁定风格/色光/比例，并给出可粘贴的图/视频 style block；附校验脚本
- **action-physics-choreography**：把空喊动作拆成受力方向与落地；附校验脚本

## Recipe / links
- 仓库：https://github.com/xuyewild/ai-video-skills
- 例：`cp -r ai-video-skills/skills/zh/visual-bible ~/.claude/skills/`
- 测试：`python -m unittest discover -s tests -v`

## Why it made the cut
来自大量返工的可执行配方 + 校验脚本；中英齐全；MIT。
