# Agent Skills Wiki

A living public wiki of high-quality, reusable **agent skills** discovered from X (Twitter).

Curated for people who build with coding agents (Cursor, Claude Code, Grok Bot, and similar). Each entry links back to the original post and summarizes what the skill does, when to use it, and why it stood out.

## Browse

- [Wiki home](wiki/Home.md)
- [Catalog](wiki/Catalog.md)
- [Hourly digests](wiki/digests/)

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
  Catalog.md       # index of all entries
  entries/         # one markdown file per skill
  digests/         # hourly scan digests
meta/
  last-scan.json   # scanner cursor / dedupe state
```

## License

Content in this repo is [CC BY 4.0](LICENSE). Linked posts remain owned by their authors.

## Maintenance

Scans run about hourly (Asia/Shanghai daytime). New finds are appended to digests and promoted into `wiki/entries/` when they clear the quality bar.
