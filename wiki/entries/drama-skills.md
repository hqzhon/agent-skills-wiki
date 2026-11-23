# drama-skills（ZenStory 短剧/漫剧十二技能）

**Tags:** short-drama, screenplay, storyboard, video, skill-pack, chinese
**Source:** [@bibitcanus](https://x.com/bibitcanus/status/2124679047879840082) · 2026-11-23
**Engagement:** 本窗提示帖 1 赞（回复 @dextune）；仓库 [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) 4,782★ / 806 forks，MIT；项目页 zenstory.ai/drama-skills

## When to use
要从一个点子或一部原著，走到分集剧本、视觉设定、分镜、图/视频提示词和成片，做 AI 短剧或漫剧。可以只跑其中某一段（已有草稿只审查、静态漫剧可以从首帧图和口播直接进制作）。

## What it does
12 个可独立安装的技能，覆盖：原著分析、对标片拆解、故事开发、分集剧本、视觉设定、生图提示词、分镜/首帧、视频提示词、确认制作、剪辑、审查，以及成片交付。其中 7 个带脚本，需要 Python 3.9+；`short-drama-edit` 与 `short-drama-breakdown` 还需要 `ffmpeg` / `ffprobe`；复杂字幕/屏字可选 Remotion（纯标题可用 ffmpeg 回退）。仓库带 CI 和中英 README。

## Recipe / links
- Repo: https://github.com/zenstory-ai/drama-skills（4,782★，MIT）
- 项目页：https://zenstory.ai/drama-skills （中文：https://zenstory.ai/zh/drama-skills）
- 安装：
  ```bash
  npx skills add zenstory-ai/drama-skills -y -g
  ```
  去掉 `-g` 则只装到当前目录；同样命令可重复执行以更新。也可按需只软链 `skills/` 下的一部分。

## Why it made the cut
高星、可安装、阶段清楚的完整短剧工作流，不是目录合集。与已收录的 [awesome-short-drama-skills](awesome-short-drama-skills.md)（精选清单 + finder）、[ai-manju-skills](ai-manju-skills.md)、[shuohao-skills](shuohao-skills.md) 互补：这里是 ZenStory 自己的十二技能包。本窗帖子互动低，按高星漏收补上。
