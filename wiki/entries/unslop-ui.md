# unslop-ui（去掉界面和图表里的 AI 痕迹）

**Tags:** design, ui, frontend, anti-slop, charts, copy, skill
**Source:** [@AlphaByPablo](https://x.com/AlphaByPablo/status/2124802475282845719) · 2026-11-23；1.0 宣布 [@fildotai](https://x.com/fildotai/status/2125620778267975773) · 2026-11-26
**Engagement:** 发现帖信号低；1.0 宣布帖本窗 166 赞 / 5 转发 / 172 收藏。仓库 [felipebasurto/unslop-ui](https://github.com/felipebasurto/unslop-ui) 现 867★ / 18 forks，MIT，技能版本 1.0.2

## When to use
agent 刚搭好的页面或仪表盘一眼能看出 AI 味：标题上的 eyebrow 小标签、无意义的 `01 //` 编号、重复标题的副标题、解释按钮的说明、装饰图标/徽章、空转的 LIVE 圆点、卡片边缘那条粗色条、给图表起「折线图：周活」这种题目。要的是删掉这些痕迹并给出改动报告，而不是整页重新设计。1.0 起也可以在 agent 刚建完或改完一屏之后自动做一次收尾。若要把 vibecoded 页面逐轮改出性格和视觉方向，用已收录的 [unslop](unslop.md)（heydamir/unslop）。

## What it does
v1.0 起变成一份约 156 行、只含指令的 `SKILL.md`（现为 1.0.2）：不再附计数脚本或加载器，把仓库链接发给 Claude Code / Cursor / Codex 即可。按编号规则清点并删除界面/图表文案里的 AI 痕迹（U1–U16、U21–U24；U23 只报告不改布局）：eyebrow、装饰编号、副标题反射、botsplaining、设计注释泄漏、无状态徽章、装饰 emoji、`Learn more →` 这类泛按钮、卡片边缘粗色条、图表垃圾墨水等。U24（边缘色条）从 1.0.1 起改为默认执行。可选 `--surface`（或口头要求一并做视觉清理）再收 U17–U20 与 U25（渐变发光、非 4/8 间距、过重字重、无差别动效、边缘对齐不一致）。可选 `--plan` 先给方案再改文件。若项目里有 `.unslop-ui/taste.md`，会先读主人的禁用/保留规则。结尾有报告：裁定、按规则的找到/已修/有意保留，以及改写过、需要你复核的字符串。不编造代码里没有的数字或功能，不改逻辑/数据；无障碍标签和真实状态相关的文案或色条会保留。

## Recipe / links
- Repo: https://github.com/felipebasurto/unslop-ui（867★，MIT）
- 技能文件：https://github.com/felipebasurto/unslop-ui/blob/main/skills/unslop-ui/SKILL.md
- 不装也能用：把仓库链接发给 agent，并指明要清理的文件，例如 `Clean up the copy in src/pages/landing.tsx with https://github.com/felipebasurto/unslop-ui`
- 仍可安装：`npx skills add felipebasurto/unslop-ui -g`
- Claude Code 插件：`claude plugin marketplace add felipebasurto/unslop-ui` 再 `claude plugin install unslop-ui@unslop-ui`
- 可选 `--surface` / `--plan`（或用对应的口头说明）

## Why it made the cut
和 2 万星的 [unslop](unslop.md) 不是同一仓库：这边更窄，专攻文案和图表里的可枚举「AI 痕迹」，默认不重做视觉方向，规则带编号。1.0 删掉脚本后更符合 Agent Skills 规范，描述里会在建完/改完界面后自行触发。本窗按 1.0.2 更新条目；867★、MIT，安装或贴仓库链接均可验证。
