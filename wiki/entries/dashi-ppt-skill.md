# Dashi PPT Skill（大师 PPT）

**Tags:** slides, pptx, html, themes, chinese, skill
**Source:** [@openagentskill](https://x.com/openagentskill/status/2121324787633156347) · 2026-11-14
**Engagement:** 发现帖本身几乎无互动；仓库 [chuspeeism/dashi-ppt-skill](https://github.com/chuspeeism/dashi-ppt-skill) 约 10.7k★ / 907 forks，AGPL-3.0

## When to use
要把文档交给 agent 做职场演示稿，并且希望在浏览器里逐页改版式和控件，再导出真正可编辑的 PPTX / PDF / HTML，而不是一堆图片幻灯片。

## What it does
`skills/dashi-ppt/SKILL.md`（约 26KB）生成带每页编辑控制台的网页演示稿：12 套视觉主题、文档声称 1020 个版式页和 8576 个可调控件，可在浏览器里改完再导出可编辑 PPTX。生成、编辑、导出都在本机完成；联网主要用于首次安装依赖和静默检查版本号。需要 Node.js 20+；导出 PPTX / PDF 需要本机 Chrome / Chromium / Edge（可用 `CHROME_PATH`）。许可是 AGPL-3.0，二次分发需注意 copyleft。

## Recipe / links
- Repo: https://github.com/chuspeeism/dashi-ppt-skill
- SKILL.md: https://github.com/chuspeeism/dashi-ppt-skill/blob/main/skills/dashi-ppt/SKILL.md
- 安装/更新：`npx dashi-ppt-skill@latest`
- 国内镜像：`npx --registry=https://registry.npmmirror.com dashi-ppt-skill@latest`
- 环境：Node.js 20+ 与 npm；导出需本机 Chrome 系浏览器

## Why it made the cut
可安装的完整 SKILL.md，演示场景清楚，高星仓库可验证；和目录里已有的模板填字类 PPT skill（如 GordenPPT、萝卜 PPT）互补，强调浏览器内编辑再导出真 PPTX。注意 AGPL-3.0。
