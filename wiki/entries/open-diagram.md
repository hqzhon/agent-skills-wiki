# open-diagram（会自检布局的架构图 / 系统图）

**Tags:** diagrams, architecture, python, svg, mcp, skill
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2125190362742374569) · 2026-11-24
**Engagement:** 本窗为技能圈盘点帖（1 赞）；仓库 [lukendeasy/open-diagram](https://github.com/lukendeasy/open-diagram) 现 373★，MIT，2026-11-24 仍在推送

## When to use
需要架构图、系统地图、分层栈、数据流、云资源图或概念图，并且希望**第一稿就能看出对不对**时用。它按字体测量标签、自动摆放，并给每个布局问题起名字（碰撞、线穿过面板等），不必先盯着图猜哪里歪了。若只要按品牌风出单文件 HTML+SVG 图表，见已收录的 [Diagram Design](diagram-design.md)。

## What it does
Python 库 + \`skills/open-diagram/SKILL.md\`。可以把简短 JSON、Mermaid 或 Python 脚本编成 SVG/PNG。若环境有 MCP 工具（\`format_guide\` / \`check\` / \`draw\` / \`describe\` / \`template\`），技能要求先 \`check\` 到 0 个问题再 \`draw\`；否则先 \`pip install -U open-diagram\` 再用本地库。另有云图标技能目录 \`skills/cloud-icons\`。站点与对比文档在 [open-diagram.dev](https://open-diagram.dev)。

## Recipe / links
- Repo: https://github.com/lukendeasy/open-diagram（373★，MIT）
- 文档/画廊：https://open-diagram.dev
- 安装库：\`pip install open-diagram\`
- 安装技能：\`npx skills add lukendeasy/open-diagram\`
- Skill: [skills/open-diagram/SKILL.md](https://github.com/lukendeasy/open-diagram/blob/main/skills/open-diagram/SKILL.md)

## Why it made the cut
可验证的库 + 可加载 skill，场景清楚，自检布局是和「让模型直接画一张 SVG」不同的配方。373★、MIT，和 Diagram Design 互补而不是重复。本窗只是盘点提到，按仓库信号补收。
