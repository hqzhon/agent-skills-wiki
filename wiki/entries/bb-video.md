# BB-Video（纯代码画出讲解片 / 产品宣传片）

**Tags:** video, motion, explainer, promo, skill
**Source:** [@dextune](https://x.com/dextune/status/2123974429700976700) · 2026-11-21
**Engagement:** 介绍帖 19 赞 / 1 转 / 23 收藏；仓库 [BubbleBrainBB/BB-Video](https://github.com/BubbleBrainBB/BB-Video) 207★，MIT。

## When to use
给一个**网站 URL**（或一个要讲清楚的主题），想让 agent 做成带旁白的产品宣传片或讲解片，并且**不用剪辑软件、不用素材库**时使用。你只需选定视觉风格，其余分镜、旁白、配音、配乐、排版和渲染前检查交给技能。

## What it does
可装 agent skill（`bb-video`）。每一帧用 HTML / SVG / canvas 按时间画出来，在 headless Chrome 逐帧渲染，音效和配乐也在代码里合成，最后用 ffmpeg 编码。支持 16:9 和 9:16，官方列出 37 种风格（白板、水墨、剪影木偶、像素、等距、上线发布动效、漫画、蓝图、拼贴等）。给 URL 时，它会抓站点文案、数据和配色，截图，并用真实 UI 和品牌色做宣传片。渲染前会检查重叠、字幕消失过早、没有依据的事实和运动问题。

## Recipe / links
- Repo：https://github.com/BubbleBrainBB/BB-Video（MIT，207★）
- 安装：
  ```
  npx skills add BubbleBrainBB/BB-Video
  ```
- 技能目录在 `skills/bb-video`。需要本机或环境里有 Chrome 与 ffmpeg；出片会跑本地渲染，先看磁盘和权限。

## Why it made the cut
场景清楚，风格表和检查步骤都写在仓库里，产出是代码绘制的成片而不是「帮我写分镜」。与已收录的 product-launch-motion、cinematic-skill 等互补（这一条强调 37 种风格 + URL 调研 + 渲染前质检）。
