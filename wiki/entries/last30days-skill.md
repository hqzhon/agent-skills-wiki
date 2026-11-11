# last30days（近 30 天全网真实讨论调研）

**Tags:** research, trends, reddit, x, polymarket, skill
**Source:** [@Gerry1723625](https://x.com/Gerry1723625/status/2120168164541809144) · 2026-11-10
**Engagement:** mvanhorn/last30days-skill ~67k★

## When to use
想快速知道一个话题、产品或人物最近 30 天在真实用户里是怎么被讨论的：选题、竞品调研、发布前后舆情、投资前看情绪。

## What it does
并行搜 Reddit、X、YouTube 字幕、TikTok、HN、Polymarket、GitHub、arXiv 等，按点赞、互动和真金白银的下注来打分，再由 agent 评审综合成带出处的摘要，而不是靠编辑推荐。Reddit / HN / Polymarket / GitHub 零配置即用，首次运行有向导解锁 X、YouTube 等来源。

## Recipe / links
- Repo: https://github.com/mvanhorn/last30days-skill（运行规格在 `skills/last30days/SKILL.md`）
- Claude Code：`/plugin marketplace add mvanhorn/last30days-skill` → `/plugin install last30days`
- 其他 50+ Agent Skills 宿主：`npx skills add mvanhorn/last30days-skill -g`；调用 `/last30days <话题>`

## Why it made the cut
场景清晰、有 SKILL.md 和多宿主安装方式，社区信号极强，适合做选题与调研的固定工具。
