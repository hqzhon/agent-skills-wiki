# svg-line-story（主题生成可离线打开的 SVG 长卷）

**Tags:** svg, animation, storytelling, illustration, python, chinese, skill
**Source:** [@lkkchenlkk](https://x.com/lkkchenlkk/status/2125154245750186486) · 2026-11-24
**Engagement:** 本窗为作者发布帖（1 赞）；仓库 [lkkchen/svg-line-story](https://github.com/lkkchen/svg-line-story) 现 0★，MIT，含示例、脚本和测试，2026-11-24 仍在推送

## When to use
只有一个主题，想做成**可以离线打开的 SVG 长卷动画**（线在生长、页面随故事撑高），而不是整页插画或视频渲染时用。核心编译只用 Python 标准库；Pillow 与 Playwright 可选。

## What it does
根目录 [SKILL.md](https://github.com/lkkchen/svg-line-story/blob/main/SKILL.md) 把 agent 定位成故事导演 + 矢量美术 + 动画编排 + SVG 工程师：从立意、分镜、原创矢量、连续贝塞尔路径到浏览器 QA。默认保持纯 SVG 主体和 SMIL 时间轴；透明 GIF 只允许做花瓣、微光、振翅等局部装饰，并可完全关闭。仓库带在线演示、\`examples/\`、\`scripts/plan_story.py\` 与 \`run_theme.py\`，以及调色板/叙事骨架约定，避免新主题去抄示范故事的开场或幕数。

## Recipe / links
- Repo: https://github.com/lkkchen/svg-line-story（0★，MIT）
- 在线示例：https://lkkchen.github.io/svg-line-story/
- 安装：\`npx skills add lkkchen/svg-line-story\`，或把含 \`SKILL.md\` 的目录拷进本地 skills
- 需要能读写工作区并运行 Python 3.10+ 的 agent。成品写到工作区 \`stories/<英文短名>/\`

## Why it made the cut
星数和互动都很低，但有可加载 \`SKILL.md\`、可离线演示、脚本和测试，使用场景独特（生长中的矢量长卷，而不是再做一个 MP4 技能）。和已收录的手绘/短片技能不重复。本窗即作者说明帖。
