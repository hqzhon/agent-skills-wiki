# equity-research（Anthropic × LSEG 股票研究快照）

**Tags:** finance, equity-research, official, lseg, mcp
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2121236226640617758) · 2026-11-14（安装步骤见[预览](https://x.com/huangcheng943/status/2121236462284996863)与[安装](https://x.com/huangcheng943/status/2121236599124156583)）
**Engagement:** 发现帖热度一般；技能位于官方仓 [anthropics/financial-services](https://github.com/anthropics/financial-services) 的 LSEG 合作插件中

## When to use
研究一只美股（或比较一致预期与实际、看估值与宏观背景）时，想把 IBES 分析师一致预期、公司基本面、历史价格和宏观指标收进同一份研究快照。没有 LSEG MCP 连接和账号授权时不要用：Skill 本身不提供行情。

## What it does
`plugins/partner-built/lseg/skills/equity-research/SKILL.md` 定义五段数据流程，再综合成投资论点：① IBES 一致预期（EPS / Revenue / EBITDA / DPS，含分析师人数与离散度）；② 近 3–5 年基本面；③ 1 年价格与收益、52 周位置、beta；④ 近 3 个月量价；⑤ 宏观（GDP、CPI、政策利率）。输出标准化表格（预期、财务、估值）和简短投资论点（建议、公允区间、多空理由、催化剂、把握程度）。这与目录里已有的 [initiating-coverage](anthropic-initiating-coverage.md) 不是同一条：前者是合作方 LSEG 数据快照，后者是官方研报首次覆盖工作流。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/partner-built/lseg/skills/equity-research/SKILL.md
- 预览（只读）：`gh skill preview anthropics/financial-services plugins/partner-built/lseg/skills/equity-research/SKILL.md`
- 安装到 Codex 用户级（`gh skill` 仍为 preview）：`gh skill install anthropics/financial-services plugins/partner-built/lseg/skills/equity-research/SKILL.md --agent codex --scope user`
- 依赖 LSEG MCP 工具：`qa_ibes_consensus`、`qa_company_fundamentals`、`qa_historical_equity_price`、`tscc_historical_pricing_summaries`、`qa_macroeconomic`
- 使用前先核对 SKILL.md、LICENSE、工具权限，并确认数据连接已授权

## Why it made the cut
官方金融仓里可核对的 SKILL.md，使用场景和数据依赖写得很清楚；补上了 initiating-coverage 之外的 LSEG 合作研究快照，而不是又一条空喊「用 AI 做股票」的帖子。
