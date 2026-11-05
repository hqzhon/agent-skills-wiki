# Dashboard Design Skill（克制、诚实的数据看板）

**Tags:** frontend, dashboard, data-viz, design, swiftui
**Source:** [@Git_Daily](https://x.com/Git_Daily/status/2118254444643266670) · 2026-11-05
**Engagement:** discovery post (low engagement); repo ~319★ · MIT

## When to use
让 coding agent 新建、重做或评审分析/营收/指标/后台类仪表盘时（Web 或 SwiftUI），避免 AI 默认生成的花哨卡片、满屏解释句子和误导性图表。

## What it does
从 127 个真实上线的看板 + Few / Tufte / Knaflic / NN/g / WCAG / Apple WWDC 图表指南提炼的设计规范：KPI 条、图表、热力图、bullet graph、对比周期、排名拆分、日期选择器、空状态、宽屏与手机布局。2.0 主打「无字化」（解释放 tooltip）、问题直接标在数据上，并以截图 QA 收尾（字数审计、显著性测试、色盲与真实数据检查）。

## Recipe / links
- Repo: https://github.com/abdiraimov-otabek/dashboard-design-skill
- 放进 Claude Code / agent skills 目录后，让 agent「用 dashboard-design 重做这个 revenue 看板，并做截图 QA」
- README 里有「Instead of → The agent builds」对照表，可当评审清单

## Why it made the cut
有 SKILL 仓库和具体规则表；使用场景清晰（看板 UI）；带前后对比截图与 QA 流程可验证；仓库 300+ 星。
