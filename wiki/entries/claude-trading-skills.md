# Claude Trading Skills（长线投资 + 波段流程包）

**Tags:** finance, trading, investing, skill-pack
**Source:** [@latentgazette](https://x.com/latentgazette/status/2121594656832000328) · 2026-11-15
**Engagement:** 发现帖为技能生态盘点中的一条（0 赞）；仓库 [tradermonty/claude-trading-skills](https://github.com/tradermonty/claude-trading-skills) 约 4804★ / 993 forks，MIT，文档站持续更新

## When to use
你是时间有限的个人投资者，核心是长线、ETF 或股息策略，并在条件合适时做有纪律的波段；希望 agent 帮你做市场回顾、风险管理、交易计划、复盘和日志，而不是把买卖交给自动信号。不适合全自动下单、外包信号或超短线刷单。

## What it does
一套 74 个 Claude skill 的流程工具箱，按区域划分，例如：市场环境（`market-breadth-analyzer`、`uptrend-analyzer`、`exposure-coach`）、核心组合（`portfolio-manager`、`us-undervalued-growth-screener`）、股息（`kanchi-dividend-sop` 等）、波段机会（`vcp-screener`、`canslim-screener`、`breakout-trade-planner`）、交易计划（`position-sizer`、`technical-analyst`），以及日历、回测、复盘和技能自身的改进流水线。仓库强调「先为自己用、再公开分享」，并写明这不是投资建议、信号服务或券商执行平台；FMP、FINVIZ Elite、Alpaca 等是可选数据/券商集成，入门路径可用公开 CSV、图表截图和本地文件。

## Recipe / links
- Repo: https://github.com/tradermonty/claude-trading-skills（~4804★，MIT）
- 文档：https://tradermonty.github.io/claude-trading-skills/
- Claude Code：克隆仓库后，把需要的技能目录（如 `skills/backtest-expert`）拷到 `~/.claude/skills/` 或项目内 `.claude/skills/`
- Claude 网页：从 [Releases](https://github.com/tradermonty/claude-trading-skills/releases/latest) 下载对应 `.skill` 资源并核对 `SHA256SUMS`，在 Settings > Capabilities 开启 Code execution and file creation 后，于 Customize > Skills 上传
- 配套（可选）：[Hermes Trading Research Agent Work Package](https://github.com/tradermonty/hermes-trading-research-agent-work-package) 提供 `/pre-market-routine` 等例行命令，仍保留人工决策门，不下单
- 相关：本 wiki 的 [Day Trader Skill pack](day-trader-skill.md) 更偏日内交易与公开数据扫描；本包更偏长线 + 有纪律波段的决策流程

## Why it made the cut
可安装的大型技能包，使用边界写得很清楚（研究/复盘，不自动下单），仓库、文档和发布包都可验证，社区信号强，且与已收录的日内交易包互补。
