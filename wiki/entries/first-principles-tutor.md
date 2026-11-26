# First Principles Tutor（用第一性原理逼你自己把概念重建出来）

**Tags:** learning, tutoring, socratic, claude, skill
**Source:** [@Ishrit_Rai](https://x.com/Ishrit_Rai/status/2125849727279436036) · 2026-11-26
**Engagement:** 介绍帖 0 赞；仓库 [IshritRai/first-principles-tutor](https://github.com/IshritRai/first-principles-tutor) 现 6★，MIT。技能正文在 `skills/first-principles-tutor/SKILL.md`（很长的完整配方）。作者称已连续打磨数月。与已收录的 [Jane Street Socratic Tutor](janestreet-agent-skills.md) 同属苏格拉底式教学，但不是同一仓库。

## When to use
你想**真正学会**某个概念，而不是让模型直接把答案讲完时用。它适用于 claude.ai（网页/移动）、Claude 桌面端和 Claude Code。不要用它当解题代写或考试作弊器——技能的设计就是不把现成答案递过来。

## What it does
把五种教学法收进一个循环：苏格拉底提问（问、提示、故意不讲）、第一性原理（拆到底座再爬回来）、发生学方法（先给出让该概念不得不出现的问题）、Proofs and Refutations（用反例逼出精确表述）、费曼技巧（闭卷复述，缺口决定下一轮）。会话还会维护进度tracker、在每一轮放一张不剧透的示意图，并用延迟、不预告的再测检查有没有真记住。

## Recipe / links
- Repo: https://github.com/IshritRai/first-principles-tutor（6★，MIT）
- 技能：https://github.com/IshritRai/first-principles-tutor/blob/main/skills/first-principles-tutor/SKILL.md
- claude.ai / 桌面端：下载仓库，把 `skills/first-principles-tutor` 文件夹单独打成 zip，在 **Customize → Skills** 里上传；并开启「Code execution / 创建和编辑文件」能力。
- Claude Code：把该技能目录复制到 Claude 的 skills 路径后重开会话。

## Why it made the cut
可安装、何时用写得很清楚，`SKILL.md` 是可执行的长配方而不是一句「请用苏格拉底法」。6★、介绍帖无互动，按可验证材料收录；和 Jane Street 官方家教包可对照，不要混成同一个。
