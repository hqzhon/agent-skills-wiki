# overfetch（前端冗余请求审计）

**Tags:** frontend, performance, network, audit, react-query
**Source:** [@drunk_vibecoder](https://x.com/drunk_vibecoder/status/2117948418085757393) · 2026-11-04
**Engagement:** 仓库 alii13/overfetch，MIT，2026-11-04 刚发布（星数尚少，按内容质量收录）

## When to use
应用「请求太多」、后端被前端打爆、撞速率限制，或想审一遍 TanStack Query / SWR / Apollo / RTK Query 的缓存与轮询行为；也适合手里有 HAR / 网络抓包要分析时。

## What it does
产出一份按严重程度排序、带证据的请求放大报告：逐行 N+1、重复请求、叠加的轮询计时器、零缓存新鲜度、整体失效、串行瀑布、全量分页、过度取数、重试浪费。每条发现附 `file:line` 或抓包证据、根因、修复模式、预期降幅和工作量；还列出「排查过但排除」的项、需要产品或后端决定的事，以及审计没覆盖到的部分。原则是正则命中只算候选，必须读代码确认；实测抓包优先于注释和文档。审计阶段不动手改，之后可按发现一条一个 PR 修。

## Recipe / links
- Repo: https://github.com/alii13/overfetch
- `SKILL.md` + `scripts/static_scan.py`（静态扫描候选）+ `references/report-template.md`（报告模板）
- 触发说法示例：「这个 app 请求太多」「后端被打爆了」「查一下我们的缓存」

## Why it made the cut
配方完整且克制（强调核验与覆盖范围说明），场景具体、可直接复用；虽然是新仓库，但 wiki 里还没有专门做前端网络请求审计的 skill。
