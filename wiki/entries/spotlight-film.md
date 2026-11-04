# Spotlight Film（Apple 发布会风格产品片）

**Tags:** video, launch-video, motion, threejs, product-demo
**Source:** [@ridemountainpig](https://x.com/ridemountainpig/status/2117844161944801298) · 2026-11-04
**Engagement:** 推文约 120 次浏览、3 收藏；仓库 ridemountainpig/spotlight-film 新建（个位数★，MIT）

## When to use
想给产品做 Keynote 式发布短片：黑色舞台、光束把内容带出、超大倾斜标题、硬切证明镜头；手上有 README、截图或录屏，想要可逐帧审阅的确定性成片。

## What it does
- 把产品简介变成渲染好的发布片，所有画面由代码生成（HTML + three.js、Playwright、ffmpeg）。
- 流程：先和你一起规划影片 → 渲染静帧供审阅 → 预览 → 输出无声 MP4（自配音乐）。
- 只用你提供的素材，不编造人物、地点或镜头。

## Recipe / links
- Repo: https://github.com/ridemountainpig/spotlight-film
- 安装：`npx skills add ridemountainpig/spotlight-film`，或把 `skills/spotlight-film` 复制到 `~/.claude/skills/`
- 示例提示：「Make a 30-second launch film for our app. Here's the README, three screenshots and a screen recording of the new editor.」
- 完整流程见仓库内 `skills/spotlight-film/SKILL.md`

## Why it made the cut
有 SKILL.md 与可看的 demo 片（open-slide、Raycast Keyboard），场景明确、MIT；虽然星数还少，但材料可验证，和 product-launch-motion / onetake 形成不同风格的发布片选项。
