# claude-drawing-skill（用代码作画，83 种画风）

**Tags:** generative-art, illustration, python, claude-code, skill
**Source:** [@warmtalent1](https://x.com/warmtalent1/status/2122280866319942140) · 2026-11-16
**Engagement:** 发现帖互动很少（0 赞 / 2 次展示）；仓库 [cloveric/claude-drawing-skill](https://github.com/cloveric/claude-drawing-skill) 现 260★ / 30 forks，MIT

## When to use
想让 coding agent **不用生图模型**、在 CPU 上用 Python 一笔一笔作画：水墨、水彩、油画厚涂、浮世绘、彩绘玻璃、像素风等；需要构图可控、同一种子可复现，或把作画过程存成逐步显现的 GIF。不是把故事文案做成手绘动画短片——那应走 [story-to-handdrawn-video](story-to-handdrawn-video.md)。

## What it does
Claude Code 技能 + 小型绘画库：83 种画风（八大类），只依赖 numpy 与 Pillow，离线、无 GPU、无 API Key。流程是先规划构图、写短场景脚本，再渲染并对照该画风的失败模式清单改 2–4 轮；每一步可保存，回放像「先素描再上色」。仓库带 91 张作画动图示例。SKILL.md 体积很大（约 740KB），把各画风剧本写进了技能文件。

## Recipe / links
- Repo: https://github.com/cloveric/claude-drawing-skill（MIT，260★）
- 安装：

```bash
git clone https://github.com/cloveric/claude-drawing-skill.git ~/.claude/skills/claude-drawing
pip install -r ~/.claude/skills/claude-drawing/requirements.txt
```

- 触发词示例：「claude绘图」「你自己画」「用代码画」，可指定画风
- 题字需要中文字体，一般能自动发现系统字体，或设 `INKPAINT_FONT`
- 用法说明：https://github.com/cloveric/claude-drawing-skill/blob/main/docs/USAGE.md

## Why it made the cut
可加载 SKILL.md + 可运行的本地库，场景和「不用生图模型」的边界都很清楚，有大量可验证示例和明确安装路径。发现帖本身几乎无互动，但仓库已有 260★ / 30 forks。与手绘故事短片技能不同，这是静帧/作画过程导向的程序化插画。
