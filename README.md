# Agent Skills Wiki

A living public wiki of high-quality, reusable **agent skills** discovered from X (Twitter).

## Skills 入口（从这里开始）

👉 **[打开完整目录 Catalog](wiki/Catalog.md)** — 所有已收录 skill 的索引表（名称、标签、来源、日期）。

也可以从这里进：

- [Wiki home](wiki/Home.md) — 收录标准与用法
- [单条详情](wiki/entries/) — 每个 skill 一份 markdown
- [Hourly digests](wiki/digests/) — 每小时扫描摘要

Curated for people who build with coding agents (Cursor, Claude Code, Grok Bot, and similar). Each entry links back to the original post and summarizes what the skill does, when to use it, and why it stood out.

## What counts as a skill here

A **skill** is a reusable multi-step recipe an agent can load: clear trigger (“use when…”), concrete steps, and preferably a shareable `SKILL.md` or equivalent write-up.

We keep:

- Original source link (X post or thread)
- Short summary in plain language
- Tags (domain, tool, language)
- Quality notes (why it made the cut)

We skip ads, empty hype, and posts with no actionable recipe.

## Layout

```
wiki/
  Home.md          # overview
  Catalog.md       # index of all entries  ← 主入口
  entries/         # one markdown file per skill
  digests/         # hourly scan digests
meta/
  last-scan.json   # scanner cursor / dedupe state
```

## Related

- [一人公司机会 Wiki](https://github.com/hqzhon/opc-opportunity-wiki) — 跨境 / SaaS 一人公司机会清单

## License

Content in this repo is [CC BY 4.0](LICENSE). Linked posts remain owned by their authors.

## Maintenance

Scans run about hourly (Asia/Shanghai daytime). New finds are appended to digests and promoted into `wiki/entries/` when they clear the quality bar.
