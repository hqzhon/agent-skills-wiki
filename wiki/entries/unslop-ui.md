# unslop-ui（去掉界面和图表里的 AI 痕迹）

**Tags:** design, ui, frontend, anti-slop, charts, copy, skill
**Source:** [@AlphaByPablo](https://x.com/AlphaByPablo/status/2124802475282845719) · 2026-11-23
**Engagement:** 发现帖信号低；仓库 [felipebasurto/unslop-ui](https://github.com/felipebasurto/unslop-ui) 767★ / 17 forks，MIT

## When to use
agent 刚搭好的页面或仪表盘一眼能看出 AI 味：标题上的 eyebrow 小标签、无意义的 `01 //` 编号、重复标题的副标题、解释按钮的说明、装饰图标/徽章、空转的 LIVE 圆点、给图表起「折线图：周活」这种题目。要的是删掉这些痕迹并给出改动报告，而不是整页重新设计。若要把 vibecoded 页面逐轮改出性格和视觉方向，用已收录的 [unslop](unslop.md)（heydamir/unslop）。

## What it does
按编号规则清点并删除界面/图表文案里的 AI 痕迹（U1–U16、U21–U25 等）：eyebrow、装饰编号、副标题反射、botsplaining、设计注释泄漏、无状态徽章、装饰 emoji、图表垃圾墨水等。可选 `--surface` 再收视觉层（渐变发光、非 4/8 间距、`font-black`、无差别动效等）。可选 `--plan` 先给方案再改文件。结尾有报告：裁定、按规则的找到/已修/有意保留，以及改写过、需要你复核的字符串。不编造代码里没有的数字或功能，不改逻辑/数据/配色/布局；无障碍标签和真实状态相关的文案会保留。

## Recipe / links
- Repo: https://github.com/felipebasurto/unslop-ui（767★，MIT）
- 不装也能用：把仓库链接发给 agent，并指明要清理的文件
- 常用安装：`npx skills add felipebasurto/unslop-ui -g`，然后 `/unslop-ui src/pages/landing.tsx`（可加 `--surface` 或 `--plan`）
- Claude Code 插件：`claude plugin marketplace add felipebasurto/unslop-ui` 再 `claude plugin install unslop-ui@unslop-ui`

## Why it made the cut
和 2 万星的 [unslop](unslop.md) 不是同一仓库：这边更窄，专攻文案和图表里的可枚举「AI 痕迹」，默认不重做视觉方向，规则带编号、有评测 fixtures。作者也写明写作规则来自 Lauren Tan 的 unslop，并和 heydamir/unslop 做过对照。767★、MIT，安装命令可验证。
