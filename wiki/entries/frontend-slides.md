# Frontend Slides（网页幻灯片 / 转 PPT）

**Tags:** slides, html, presentation, skill, claude-code
**Source:** [@CatOnShift](https://x.com/CatOnShift/status/2125438934117151001) · 2026-11-25
**Engagement:** 本窗介绍帖互动为 0；仓库 [zarazhangrui/frontend-slides](https://github.com/zarazhangrui/frontend-slides) 现 32,869★，MIT。最新正式标签 v2.1.0（2026-05-26），最近推送停在 2026-06-23。

## When to use
要用编码助手做一份能在浏览器打开的 16:9 网页演示，或把已有 PowerPoint 转成网页幻灯片（保留文字和图片）时用。成品是单文件 HTML（内嵌 CSS/JS），不必再跑 npm 打包。不要用它做会在手机上重排的响应式页面——画布按 1920×1080 缩放，必要时加黑边。

## What it does
先问用途和内容，再给出多种视觉预览让你挑，然后才生成完整演示并在浏览器打开（避免一上来就是白底紫渐变）。也可把 `.pptx` 转成网页。可选 Bold 模板包。导出 PDF 是静态截图，动画不会保留；发布到网址按文档需要 Node.js 和 Vercel 账号。

## Recipe / links
- Repo: https://github.com/zarazhangrui/frontend-slides（32,869★，MIT）
- Claude Code 插件（请分成两条消息，不要一次贴两行）：

```
/plugin marketplace add https://github.com/zarazhangrui/frontend-slides
/plugin install frontend-slides@frontend-slides
```

  之后用 `/frontend-slides:frontend-slides`。也可 git clone 到 `~/.claude/skills/frontend-slides`，命令则为 `/frontend-slides`。
- 其他能读写文件并执行命令的编码助手，把仓库交给它并让它按 `SKILL.md` 执行即可。转 PPT 需要本机 Python 与 `python-pptx`；导出 PDF 需要 Node.js，脚本会按需安装 Playwright。

## Why it made the cut
高星漏收：可加载 SKILL.md、预览再成稿的流程清楚，32,869★、MIT。和目录里已有的原生 PPTX 技能（[Dashi](dashi-ppt-skill.md)、[GordenPPT](gorden-ppt-skill.md)、[萝卜 PPT](luobo-ppt.md)）互补——这边交付的是可离线打开的网页幻灯片。仓已数月未推送，装前以当前 README 为准。
