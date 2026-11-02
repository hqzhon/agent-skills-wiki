# InvestSkill（美股分析框架合集）

**Tags:** finance, investing, stock-analysis, skill-pack
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2117203439176577339) · 2026-11-02
**Engagement:** 仓库 yennanliu/InvestSkill，~272★，MIT，带 CI 测试与文档站

## When to use
读美股 10-K / 10-Q、做个股初筛或估值时，希望 agent 按固定框架把关键数字、会计质量、现金流、债务、风险因素和管理层表述理一遍，而不是只看营收和 EPS。

## What it does
34 个结构化分析框架（如 `financial-report-analyst` 财报初读、`stock-eval` 给出 Piotroski 分数 / ROIC / 护城河评级等），纯 markdown，无需 API key 或数据订阅。要求注明数据日期与出处；输出是研究信号，不是买卖建议，结论需回原文核实。

## Recipe / links
- Repo: https://github.com/yennanliu/InvestSkill · 文档：https://yennj12.js.org/InvestSkill/
- 安装：`curl -fsSL https://raw.githubusercontent.com/yennanliu/InvestSkill/main/install.sh | bash -s -- -a claude`（`-a` 可换 cursor / copilot / gemini / codex / opencode / any；建议先读 install.sh 再执行）
- Claude Code 会写入 `.claude/skills/<skill>/SKILL.md` 作为斜杠命令
- 用法示例：`Evaluate AAPL using the stock-eval framework`

## Why it made the cut
配方具体、使用场景明确、仓库可验证且有测试和中文文档；与 hithink-finance、money-snapshot 互补，偏美股基本面研究。
