# 「动」悉万物（z-dongxi：把内容做成会动的解析图）

**Tags:** visualization, svg, animation, explainer, chinese, skill
**Source:** [@27huff](https://x.com/27huff/status/2126231552476778636) · 2026-11-27
**Engagement:** 使用分享帖 1 赞，并给出安装与一次 Git 分支概念动图的完整提示词；技能位于已收录过单条技能的包 [tjxj/z-skills](https://github.com/tjxj/z-skills)（现 684★）。仓库根目录没有 LICENSE 文件，收录时按上游现状标明。

## When to use
要把一段有先后、因果、流动、占比或结构关系的内容，做成**会动的解析图**（单行内联 SVG，可直接贴进公众号，也可导出 PNG / GIF / MP4），又不想自己写 Mermaid 或调动画时用。不适合主节点超过 9 个的大架构、要读精确数值的大表，或需要点击交互的图。它是 `tjxj/z-skills` 包里的一条技能，和已收录的 [wx-downloader / z-video-downloader](z-video-downloader.md) 同包但用途不同。

## What it does
技能名 `z-dongxi`。工作流是：先判断适不适合 → 写清「什么在动」→ 选图型和风格 → 渲染 → 检查 → 导出。内置约 35 种图型（过程类 13 种，如流程、时序、状态机、漏斗、Git 分支；数据与结构类 18 种，如环形占比、桑基、甘特、ER、雷达；层次与立体类 4 种），约 27 种风格（瑞士网格、Excalidraw 手绘、工程蓝图、像素街机、水墨朱印等），以及 5 种画幅（默认 3:4，另有 9:16、1:1、4:3、16:9）。图型底部可以加一排会动的小物件。使用者不必自己选图型；拿不准时默认 `flow`。

## Recipe / links
- 技能目录：https://github.com/tjxj/z-skills/tree/main/z-dongxi
- 包：https://github.com/tjxj/z-skills（684★；根目录未见 LICENSE）
- 安装：
  ```bash
  npx skills add tjxj/z-skills --skill z-dongxi
  ```
  按安装器选择目标 agent。也可以克隆后把 `z-dongxi` 目录拷进 agent 的 skills 目录。
- 技能文件：`z-dongxi/SKILL.md`

## Why it made the cut
有非常具体的配方（图型/风格/画幅和强制分步），场景清楚（科普、课件、公众号里的动态示意图），材料可核。本窗是使用者演示而不是作者发帖，但上游包已有社区星标，且 wiki 此前只收过同包的视频下载技能，这条可视化技能值得单列。使用前请自行确认许可和依赖（渲染/导出脚本以该目录说明为准）。
