# idea-generation（Anthropic 金融选股思路）

**Tags:** finance, investing, research, screening, official, skill
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2119785822472003892) · 2026-11-09
**Engagement:** 发现帖 · anthropics/financial-services · Apache-2.0 · ~41k★

## When to use
需要系统地找新的多/空投资思路：跑价值 / 成长 / 质量等量化筛选、做主题扫描，或「pitch me something」。仅用于研究学习，不是投资建议，也不执行交易。

## What it does
官方 SKILL.md 流程：先问清方向、市值、行业、风格、地域、主题 → 按风格套量化筛选条件（如价值：P/E 低于行业中位、FCF 收益率 >5%；成长：营收 >15% YoY 等）→ 叠加主题研究与模式识别 → 产出候选清单。本身不带行情，需要你接入的数据源/连接器。

## Recipe / links
- Skill: https://github.com/anthropics/financial-services/blob/main/plugins/agent-plugins/market-researcher/skills/idea-generation/SKILL.md
- 预览：`gh skill preview anthropics/financial-services plugins/agent-plugins/market-researcher/skills/idea-generation/SKILL.md`（GitHub CLI ≥2.90，`gh skill` 仍为 preview）
- 安装到 Codex 用户级：`gh skill install anthropics/financial-services plugins/agent-plugins/market-researcher/skills/idea-generation/SKILL.md --agent codex --scope user`
- 同仓库另见 [anthropic-comps-analysis](anthropic-comps-analysis.md)

## Why it made the cut
官方、Apache-2.0、步骤和筛选阈值写得具体，安装命令可复制；补齐金融研究链条的「找思路」一环。
