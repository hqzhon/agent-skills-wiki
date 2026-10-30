# 史鉴人生抉择（shiji-tongjian-decisions）

**Tags:** decision-making, history, chinese, evaluation, skill
**Source:** [@zhuy1043](https://x.com/zhuy1043/status/2116049614302220639) · 2026-10-30
**Engagement:** author launch (new account); material = zhuyep/shiji-tongjian-decisions MIT + evals/examples（stars still thin）

## When to use
When facing **去留 / 转型 / 合作 / 承诺** 类进退两难，希望 agent 把问题放回《史记》《资治通鉴》的决策现场：有出处、有反例、有适用边界，而不是鸡汤类比。

## What it does
Source-grounded historical decision skill：对照历史路径与结果，标出反事实与现代需核实事项；引文可离线核验（`python3 skills/.../scripts/corpus.py verify`），找不到出处就明说缺口。仓库含完整示例、evals、中英 README；不装也能先读公开推演再决定是否安装。

## Recipe / links
- Repo: https://github.com/zhuyep/shiji-tongjian-decisions
- Install: `npx skills add zhuyep/shiji-tongjian-decisions --skill shiji-tongjian-decisions`
- Preview example: `examples/promotion-decision.zh-CN.md`
- Skill: `skills/shiji-tongjian-decisions/SKILL.md`

## Why it made the cut
Unusual but executable niche: recipe + offline citation verify + public worked example. Community signal still thin—keep an eye on eval quality over star count.
