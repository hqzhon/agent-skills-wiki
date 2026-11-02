# svg-diagram（Bybit 开源的 SVG 画图规范 + 检查器）

**Tags:** diagram, svg, architecture, flowchart, lint, skill
**Source:** [@tantanyuli](https://x.com/tantanyuli/status/2117098372071092456) · 2026-11-02
**Engagement:** 仓库 bybit-exchange/svg-diagram，~643★，MIT

## When to use
让 Claude Code / Cursor / Codex 画架构图、流程图、时序图、数据流图或生命周期图，并以 SVG 放进文档，但常被「连线歪、文字溢出、中文乱码、元素重叠」折磨时。

## What it does
`SKILL.md` 给 agent 一套统一的手写 SVG 家规：按字体计算框高、明确连线与箭头位置、配色体系等版式算术。附一个零依赖 Node 检查器 `svg-lint`，对最终 SVG 跑 12 项检查（字体、留白、重叠、转义等），lint 通过才算画完。仓库里有 10 张示范图，每张对应一条规则。

## Recipe / links
- Repo: https://github.com/bybit-exchange/svg-diagram
- 安装：`npx skills add bybit-exchange/svg-diagram -g`（去掉 `-g` 装到当前项目）
- 检查：`node ~/.claude/skills/svg-diagram/tools/svg-lint/bin/svg-lint.mjs diagram.svg`
- 只要规范文本也可只拷 `SKILL.md`，但会失去 lint 闸

## Why it made the cut
配方具体（版式规则 + 可执行检查器做验收闸），场景高频，有厂商级仓库和示例；与 stack-diagram 互补。
