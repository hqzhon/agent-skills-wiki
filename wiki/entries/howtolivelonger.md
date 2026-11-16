# HowToLiveLonger（程序员延寿指南 Skill）

**Tags:** health, evidence, longevity, skill
**Source:** [@huangho75845189](https://x.com/huangho75845189/status/2121859020021805153) · 2026-11-15
**Engagement:** 3 likes / 3 replies · 仓库 [geekan/HowToLiveLonger](https://github.com/geekan/HowToLiveLonger) 现 36108★，Unlicense

## When to use
想就饮食、运动、睡眠或日常习惯问「研究怎么说」，并希望 agent 先查这份循证数据集再给可执行建议，而不是凭训练语料随口劝你。

## What it does
在已有的《程序员延寿指南》知识库上加了一条 agent skill。技能会下载并阅读仓库里的 `data/evidence.json`，按问题匹配 `records`，读 `finding` / `action` / `grade` / `effect` / 人群与限制，并用 `sources[].url` 链回原论文。`originalClaim` 只是历史表述，不是当前结论。数据集覆盖不到的问题必须直说。指南本身整理了数十项来自 NEJM / Lancet / BMJ 等期刊的研究，支持多语言在线阅读。

## Recipe / links
- Repo: https://github.com/geekan/HowToLiveLonger（36108★，Unlicense）
- 在线阅读：https://geekan.github.io/HowToLiveLonger/
- 安装：`npx skills add geekan/HowToLiveLonger --skill howtolivelonger`
- Skill 正文：仓库 `skills/howtolivelonger/SKILL.md`（会拉取 `evidence.json`，需要网络）

## Why it made the cut
高星、对公众领域友好的许可证，以及一条可安装、有明确数据源的 SKILL.md：先查证再回答，不是把长寿建议写成空口号。技能本身很短，价值主要在那份可核对的证据库。
