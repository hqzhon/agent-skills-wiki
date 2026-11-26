# Seed Skill（11 个技能：从想法跑到种子轮）

**Tags:** fundraising, startup, pitch, investors, skill-pack
**Source:** [@ncote90](https://x.com/ncote90/status/2125757224983113972) · 2026-11-26
**Engagement:** 介绍帖 0 赞 / 1 收藏（帖内为视频，未直接贴仓库）；仓库 [Jakeschincariol/seed-skill](https://github.com/Jakeschincariol/seed-skill) 现 261★ / 54 forks，MIT。仓库创建于 2026-11-01，之后未见新的推送。

## When to use
创始人要用 agent 跑**种子轮**准备时用：竞品差评调研、找匹配投资人、写商业计划与路演稿、财务模型、条款解读、资料室和月报。外联邮件和日历邀请必须你批准后才发出。这不是法律、税务或投资建议；条款技能会标出应交给律师看的地方。和已收录的 [fundraising](fundraising-skill.md)（startup / LP / M&A 三条 track，另一作者）不是同一包。

## What it does
11 个技能，产物都落在项目里的 `seed/` 目录，后面的技能接着前面的结果用：

| 命令 | 作用 |
| --- | --- |
| `/seed-scout` | 从竞品 App Store 差评里找痛点（最多约 500 条最新评论） |
| `/seed-investors` | 按公开来源和 SEC Form D 给投资人排序 |
| `/seed-market` | 自上而下 / 自下而上的 TAM / SAM / SOM，输入都带来源 |
| `/seed-model` | 36 个月收入、消耗、runway 和盈亏平衡 |
| `/seed-plan` | 商业计划（含交叉核对过的单位经济） |
| `/seed-deck` | 10 页路演稿，可演示或打成 PDF |
| `/seed-closer` | 起草个性化开发信，经你批准后才发送，并跟进约 call |
| `/seed-coach` | 按你的数字和竞品模拟投资人提问 |
| `/seed-terms` | 用白话读 SAFE / 条款清单，算稀释，标出该问律师的条款 |
| `/seed-dataroom` | 搭投资人资料室并列出缺件 |
| `/seed-updates` | 写给投资人（和说了 not now 的人）的月报 |

工具是零第三方依赖的 Python 3.8+ 脚本，读 App Store 搜索/评论和 SEC EDGAR 等公开数据。Closer 走你自己的 Gmail / Calendar 连接器，需将发送工具设为审批，有每日上限和退订句。SEC 检索需要按要求自报身份：在 `seed/config.json` 的 `sec_user_agent` 或环境变量 `SEC_USER_AGENT` 里写上姓名和邮箱。

## Recipe / links
- Repo: https://github.com/Jakeschincariol/seed-skill（261★，MIT）
- 在 Claude 里粘贴仓库链接并说 `install skill`
- Claude Code 插件：`/plugin marketplace add Jakeschincariol/seed-skill` 后 `/plugin install seed-skill@seed-skill`（命令会带 `/seed-skill:` 前缀）
- 复制到 `~/.claude/skills/` 或项目 `.claude/skills/` 可得到不带前缀的 `/seed-scout` 等命令
- 无 Claude Code 时，也可把单个 `SKILL.md` 贴进对话当模式用（会失去 Python 工具）

## Why it made the cut
11 个可加载技能、步骤和护栏（外联需批准）写得很具体，MIT，和已有融资技能不重复。介绍帖没贴链接，本窗按仓库核对后收录。仓在 11-01 创建后尚未再推送，使用时留意是否仍适用当前 Claude 插件格式。
