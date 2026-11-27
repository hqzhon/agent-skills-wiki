# 郑希观点库（zhengxi-views，可溯源的基金经理投研技能）

**Tags:** finance, funds, research, chinese, skill
**Source:** [@bkdgiffug](https://x.com/bkdgiffug/status/2126128372493287549) · 2026-11-27
**Engagement:** 介绍帖 5 赞 / 3 收藏；仓库 [lyra81604/zhengxi-views](https://github.com/lyra81604/zhengxi-views) 现 1,778★。代码与文档为 MIT；`references/corpus/` 与基金数据是郑希、易方达、天天基金等的公开披露内容，版权归原权利人，仅供研究学习。仓最近推送到 2026-10-12，自带快照可能需用脚本刷新。

## When to use
想查 **易方达基金经理郑希** 对某个行业/主题/个股「本人公开说过什么」、了解他的选股方法、把表态和真实持仓对照，或按他的框架给任意公募基金做对比/评分时用。不要把它当成买卖建议，也不要把它的推演当成郑希本人的最新观点。

## What it does
根目录 `SKILL.md` 约定：回答必须能溯源到原文（哪一年、哪一篇、原话是什么）；语料没直接谈过的主题，可以用从原文蒸馏、且每条都有原话佐证的方法框架推演，但必须在首句声明这不是他本人的表述。三块材料都在 `references/`：2012–2026 公开观点语料、方法框架、他管理过的 8 只基金真实快照（持仓/净值/业绩/规模），以及约 2.7 万只基金的列表，可按需抓取做对比和六维评分。纯检索不需要额外依赖；实时抓取/评分需要 `pip install -r requirements.txt`（requests / beautifulsoup4 / lxml）并联网。脚本要求一次只跑一条朴素的 python 命令，避免 `cd`、管道和重定向触发确认框。也提供腾讯 WorkBuddy 的 `skill.yml`。

## Recipe / links
- Repo: https://github.com/lyra81604/zhengxi-views（1,778★；代码 MIT，语料版权归原披露方）
- 郑希基金经理主页（仓库标注）：https://www.efunds.com.cn/manager/462.shtml
- Claude Code 安装：
  ```bash
  git clone --depth 1 https://github.com/lyra81604/zhengxi-views.git
  mkdir -p "$HOME/.claude/skills/zhengxi-views"
  cp -R zhengxi-views/SKILL.md zhengxi-views/README.md zhengxi-views/references zhengxi-views/scripts "$HOME/.claude/skills/zhengxi-views"/
  ```
  然后完整重启 Claude Code。WorkBuddy 把仓库放进它的 `skills/` 目录即可（已附 `skill.yml`）。
- 可选：在个人机器的 `~/.claude/settings.json` 里为 `Bash(python:*)` / `Bash(python3:*)` 放行，以减少逐步确认（会放行所有 python 命令，用完可删）。

## Why it made the cut
可加载技能，使用场景和「不杜撰、推演与原话分开、非投资建议」的边界写得很清楚，有原文语料、方法框架和真实基金数据，星标也不低。本窗有专门介绍帖。数据快照不是实时的，全市场抓取还依赖第三方公开页面，用前先看仓库的边界说明。
