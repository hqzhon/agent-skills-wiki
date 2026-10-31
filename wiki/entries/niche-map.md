# niche-map

**Tags:** research, product-strategy, market-gaps, python, clustering, skill
**Source:** [@jmdevilleros](https://x.com/jmdevilleros/status/2116166161662411221) · 2026-10-31
**Engagement:** new (0★); 6-post thread with a worked case on 144 MCP servers / agent skills

## When to use
想回答「这个市场缺什么？」而不靠拍脑袋：给产品、App、游戏、服务、工具或出版物找**空白生态位**，并在动手前验证这个空白是真需求还是海市蜃楼。

## What it does
一个领域无关的研究方法（SKILL.md 步骤 0–7）+ Python 管线：收集约 50–150 个真实条目，按书面 rubric 在 8–15 个维度上编码，盲重编码检查一致性（Cohen's kappa），再做 Ward 聚类、PCA、密度/组合空白检测，产出候选点子，最后用 mirage test 对外验证并按模板写报告。

## Recipe / links
- Repo: https://github.com/jmdevilleros/niche-map（SKILL.md 带 `name: niche-map` frontmatter）
- 用法：把文件夹放进 agent 的 skills 目录；`python niche_core.py --items items.csv --config config.json --out out/x`；`recode_check.py sample|agree`；`templates/report_template.md`
- 真实案例：`examples/mcp-skills/WALKTHROUGH.md`（144 个 MCP/技能 → 9 个候选空白，仅 1 个存活）

## Why it made the cut
完整可执行的方法论 + 工具 + 真实走查，有明确停手/验证环节；星数为零，作为小众但扎实的研究类技能收录。
