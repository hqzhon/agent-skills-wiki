# Jane Street Socratic Tutor（官方）

**Tags:** official, education, socratic, tutoring, skill-pack
**Source:** [@RoundtableSpace](https://x.com/RoundtableSpace/status/2119380660288999692) · 2026-11-08
**Engagement:** 40 likes / 2 reposts / 7 replies / 27 bookmarks · janestreet/agent_skills · 24★ · MIT

## When to use
你明确想被教、被提问或被练到掌握某个主题（「teach me / tutor me / quiz me / drill me / help me master」），而不是只要一句解释。一次性的「explain X / what is X」不要启动它。

## What it does
Jane Street 官方 `agent_skills` 仓库目前收录的技能是 **socratic-tutor**：先用 3–5 道题摸清起点，把主题拆成 4–10 个技能点并按 0–5 打分，一次只问一个问题，穿插间隔复习，最后做综合测验。答错不直接给答案，而是收窄提问；升档必须在至少两次独立检查里真正做对。聊天机器人也可以把 `SKILL.md` 正文贴进对话使用。

## Recipe / links
- Repo: https://github.com/janestreet/agent_skills （24★, MIT）
- Skill 正文: https://github.com/janestreet/agent_skills/blob/master/socratic-tutor/SKILL.md
- 把 `socratic-tutor/` 拷进 agent 的 skills 目录，然后说「teach me [主题]」
- 会话中可用：`show progress` / `harder` / `easier` / `just tell me` / `save state` / `resume from:`

## Why it made the cut
官方组织仓、完整 SKILL.md、诊断→技能图→苏格拉底提问→间隔复习→终考的流程写得很清楚，不是「Jane Street 开源了交易机器人」类 Titling。
