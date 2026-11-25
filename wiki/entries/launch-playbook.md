# Launch Playbook

**Tags:** product-hunt, launch, marketing, skill-pack
**Source:** [@giangptx](https://x.com/giangptx/status/2125486722406617583) · 2026-11-25
**Engagement:** 本窗为作者开源帖（0 赞）；仓库 [ptrgiang/launch-playbook](https://github.com/ptrgiang/launch-playbook) 现 0★，MIT，含 8 个技能和顶会发布语料。

## When to use
要让编码 agent 按同一套清单，帮你准备 Product Hunt（或同类目录站）发布时用：写 tagline、Maker 评论、图库规划、跨平台文案，并对照同类目头部发布找模式。这是发布筹备 playbook，不是成片/宣传视频技能。

## What it does
把发布工作区做成可审阅的 Markdown / JSON。先复制 `templates/` 并填写 `launch.json`，再让 agent 跑技能。八个技能：`launch-checklist`、`analyze-category`、`draft-taglines`、`write-maker-comment`、`review-launch-page`、`draft-crossposts`、`suggest-replies`、`postmortem`。`docs/` 写机制和失败模式，`data/` 放已分析的头部发布语料；`analyze-category` 会优先抽样语料，再补线上调研，并要求模式有证据。

## Recipe / links
- Repo: https://github.com/ptrgiang/launch-playbook（0★，MIT）
- 安装：`npx skills add ptrgiang/launch-playbook`，或按 README `git clone` 后把 `templates/` 拷成自己的 launch 目录
- 技能目录：https://github.com/ptrgiang/launch-playbook/tree/main/skills

## Why it made the cut
场景清楚（独立开发者做目录站发布），8 个可加载 SKILL.md、清单和语料都在仓库里，MIT。星数和帖子互动都很低，按完整配方收录，不是凭热度。
