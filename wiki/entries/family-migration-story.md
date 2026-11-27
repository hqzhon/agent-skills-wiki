# 家族迁徙故事（family-migration-story：族谱做成有声地图纪录片）

**Tags:** genealogy, video, remotion, research, turkish, skill
**Source:** [@RoundtableSpace](https://x.com/RoundtableSpace/status/2126213182415114590) · 2026-11-27
**Engagement:** 介绍帖 35 赞；原作者 [@fkadev](https://x.com/fkadev) / GitHub [`f`](https://github.com/f) 的仓库 [f/family-migration-story](https://github.com/f/family-migration-story) 现 95★（2026-11-26 新建），MIT。帖中附作者自家约 12 分钟成片演示。

## When to use
手头有族谱材料（土耳其 e-Devlet「上下代血缘」PDF、MyHeritage / Ancestry / FamilySearch 的 GEDCOM，或手写名单），想让 agent 按祖先居住地做**带出处的历史调研**，并生成 HTML 报告和**土耳其语旁白的迁徙地图视频**时用。它按地点和年代检索档案与二次文献，不是通用「讲家史」提示词。视频链路在 macOS 上开发验证；非土耳其语用系统 `say` 发音。

## What it does
Claude Code 的 skill / plugin，多步流水线大致是：

1. 解析族谱输入，整理每个人到过的地点和年份
2. 写出研究档案 `research/dossier.json`：每个地点在家族居住年份里发生过什么，来源包括奥斯曼档案目录、年鉴、人口普查、Wikidata、OpenAlex / Crossref / DergiPark 论文，以及 Internet Archive / HathiTrust 等数字化书籍。每条发现带出处和置信度
3. 生成 HTML 报告（起源分布、代际人物、当时与今日对照、家族事件与世界事件时间线、开放问题、参考文献）
4. 用 Remotion 渲染地图视频：父母两系合到一条时间线，画出迁徙路线和时期照片，并编入战争、条约、人口交换、姓氏法一类历史事件。土耳其语旁白在本地用 [yazgi-tts](https://huggingface.co/erkamk/yazgi-tts-1) 合成

作者建议用 Claude Opus 5.5、effort `xhigh`，因为步骤长、工具调用多。示例图中的人物是虚构的，地点、日期和来源是真实的。

## Recipe / links
- Repo: https://github.com/f/family-migration-story（95★，MIT）
- 安装（Claude Code plugin）：
  ```bash
  claude plugin marketplace add f/family-migration-story
  claude plugin install family-migration-story@family-migration-story
  ```
  或在会话里 `/plugin marketplace add f/family-migration-story` 后 `/plugin install family-migration-story@family-migration-story`，再 `/reload-plugins` 或重启。也可以只拷技能目录：
  ```bash
  git clone https://github.com/f/family-migration-story.git && cp -R family-migration-story/skills/family-migration-story ~/.claude/skills/
  ```
- 依赖：始终需要较新的 Claude Code 并开启网页搜索；读 e-Devlet PDF 需要 [uv](https://docs.astral.sh/uv/)；研究报告需 Python 3.10+（标准库即可）；出视频需 Node.js 20+、ffmpeg/ffprobe、uv，以及约 5 GB 磁盘（首次会下载 yazgi-tts ~1.2 GB、faster-whisper ~0.5 GB 和 Remotion 所用浏览器）
- 技能路径：`skills/family-migration-story/SKILL.md`

## Why it made the cut
有明确输入、可核来源的调研步骤和可安装 SKILL.md，输出是报告加 Remotion 成片，不是空喊「做家史」。仓库虽新，但作者是知名开源开发者，介绍帖有互动，配方完整。注意历史叙述仍需人工核对；视频和土耳其语音链路对环境和磁盘要求不低。
