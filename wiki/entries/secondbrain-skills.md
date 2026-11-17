# secondbrain-skills（Obsidian 第二大脑技能包）

**Tags:** obsidian, knowledge-base, wiki, ingest, skill-pack
**Source:** [@BeromArtDev](https://x.com/BeromArtDev/status/2122510557781627344) · 2026-11-17
**Engagement:** 发现帖为回复、互动很低；仓库 [GoBeromsu/secondbrain-skills](https://github.com/GoBeromsu/secondbrain-skills) 现 0★，MIT；作者自称仍在建设

## When to use
让 agent 把 Obsidian 库当第二大脑用：收录来源、原文留存、编译进 wiki、带引用作答；或多个 agent 同时写库时，需要按职责分包（采集、入库、校验、可视化）以免互相覆盖。已有官方 [Obsidian Skills](obsidian-skills.md) 做 CLI/Markdown/Bases/Canvas 时，这是偏「知识库流水线」的社区包。

## What it does
`skills/` 下约 20 个互相独立的包（各有一份 `SKILL.md`，无根调度器、无共享运行时），包括 `ingest` / `capture` / `inbox` / `query` / `verify` / `lint` / `audit` / `obsidian-cli` / `obsidian-visualize` 以及若干写作与档案原则技能。原则是：先原样保存 Raw 笔记，只写任务授权的目标路径，并区分解析成功与真正写入。提供 Claude Code / Codex 等 marketplace 安装方式；静态校验用 `claude plugin validate . --strict`，作者声明这还不是运行时加载验证。不要安装文档点名的 `v0.1.0` Hermes 标签。

## Recipe / links
- Repo: https://github.com/GoBeromsu/secondbrain-skills （MIT）
- Claude Code: `claude plugin marketplace add GoBeromsu/secondbrain-skills`，再 `claude plugin install secondbrain-skills@secondbrain-skills`
- Codex: `codex plugin marketplace add GoBeromsu/secondbrain-skills`，再 `codex plugin add secondbrain-skills@secondbrain-skills`
- 无插件注册表的 agent（Cursor 等）按各自文档导入 `skills/<name>/`
- 部分可视化/格式技能改写或参考了官方 obsidian-skills 等上游，详见仓库 NOTICE；安装前读各包 `SKILL.md`

## Why it made the cut
有明确使用场景和可检查的多份 `SKILL.md`，与官方 Obsidian 包互补。仓库还很新、几乎没有社区信号，且作者标明静态校验不等于已实测加载，按早期社区包收录，安装前需要自己审阅。
