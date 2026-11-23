# vela-agent-skills（LuxAlgo 官方图表库技能包）

**Tags:** official, charts, trading, finance, typescript, skill-pack
**Source:** [@hisevenih](https://x.com/hisevenih/status/2124724649443656039) · 2026-11-23
**Engagement:** 发现帖 20 赞；仓库 [LuxAlgo/Vela](https://github.com/LuxAlgo/Vela) 1,378★ / 286 forks，Apache-2.0；本窗强调其中的 agent skills 与 `llms.txt`

## When to use
要用编码 agent 做金融图表网页或图表应用：K 线/网格图、接币安等行情源、写 Vela 指标、用绘图工具、做插件，或升级已有的 Vela 集成。没有这套技能时，模型容易按过时 API 瞎编。

## What it does
LuxAlgo 开源图表库 Vela 在仓库里带了 6 个可安装 skill，并配有 `llms.txt`：
- `building-vela-charts`：用 `VelaWorkspace` 或底层 `Vela` 搭完整图表或多图网格，接离线 K 线或数据源（Binance / Coinbase / Hyperliquid / 自建），可挂 Pine Script 指标（`@luxalgo/vela-pinets`）
- `using-vela-data-providers`：接入数据源
- `adding-vela-indicators`：添加指标
- `using-vela-drawing-tools`：绘图工具
- `extending-vela-with-plugins`：插件扩展
- `upgrading-vela`：升级已有集成

## Recipe / links
- Repo: https://github.com/LuxAlgo/Vela（1,378★，Apache-2.0）
- Skills 目录：https://github.com/LuxAlgo/Vela/tree/main/skills
- 安装：`npx skills add LuxAlgo/Vela`
- 另有 `llms.txt` 供 agent 阅读库的结构与入口

## Why it made the cut
不是空喊「给库写了 skill」：6 个 SKILL.md 分工清楚，安装命令可验证，官方库本身星数和 forks 都够。适合做带实时行情的图表页，避免模型对着旧文档编 API。
