# 书脉（weread-atlas）

**Tags:** reading, weread, obsidian, knowledge-map, chinese, skill
**Source:** [@Charles77xixi](https://x.com/Charles77xixi/status/2119002644002058546) · 2026-11-07
**Engagement:** 30 likes / 2 reposts / 58 bookmarks · anneheartrecord/weread-atlas · 6★ · MIT

## When to use
微信读书里攒了大量划线和想法，但笔记按书存放、几乎不再回头看；你希望按主题重组，并生成一张能看出跨领域联系的知识地图。

## What it does
从微信读书官方接口拉取你自己的划线与想法，在 Obsidian 里写成「一书一篇 + 一主题一卡片」：卡片上的观点都链回出处，主题之间写明为什么相连，最后渲染本地网页（知识环、脉络栏、阅读统计和书架）。脚本只做拉数据、写文件、渲染页面；归纳领域/主题/关系交给你的 agent，主题方案会先给你确认再落盘。只需 Python 3.9+，无第三方依赖。

## Recipe / links
- Repo: https://github.com/anneheartrecord/weread-atlas （6★, MIT）
- 演示: https://www.charles-cheng.com/books
- 先装微信读书官方 skill（`Download https://cdn.weread.qq.com/skills/weread-skills.zip and install the skill`），在 https://weread.qq.com/r/weread-skills 取 `wrk-` API Key，`export WEREAD_API_KEY=...`
- 克隆到 skills 目录，例如 `git clone https://github.com/anneheartrecord/weread-atlas ~/.claude/skills/weread-atlas`
- 对 agent 说：「把我微信读书的笔记按主题整理进 Obsidian，再画一张我的知识地图。」之后说「更新书脉」做增量同步
- 完整流程见仓库 `SKILL.md`；数据只写本机 vault，分享页面前可让 agent 做隐私检查

## Why it made the cut
原作者把自己近 1.5 万条划线、370 本书的整理流程做成可安装 skill：有明确场景、确定性脚本 + agent 归纳、SKILL.md 和可访问的演示站。
