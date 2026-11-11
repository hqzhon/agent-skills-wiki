# Humanizer（blader，去 AI 写作痕迹）

**Tags:** writing, humanizer, editing, english, skill
**Source:** [@cryptofz66](https://x.com/cryptofz66/status/2120038004303778242) · 2026-11-10
**Engagement:** blader/humanizer ~67k★ · MIT

## When to use
让 AI 写的英文文本读起来像人写的、但不改变内容：发布公告、文档、邮件、帖子。明确不以绕过 AI 检测器为目标。

## What it does
基于 Wikipedia「Signs of AI writing」检查 26 种模式，优先处理五大破绽：「不是 X 而是 Y」、一句话收尾（Let that sink in）、伪深刻格言、铺垫式开场（Here's the thing）、和假想对手争论。README 给出前后对比，并引用一次 16/16 的盲测偏好结果（issue #229）。

## Recipe / links
- Repo: https://github.com/blader/humanizer
- Claude Code：`/plugin marketplace add blader/humanizer` → `/plugin install humanizer@humanizer`；Codex：`npx skills add blader/humanizer --global --agent codex`；调用 `/humanizer`
- 中文改编版见 [Humanizer-zh](humanizer-zh.md)；同类见 [ste80-humanizer](ste80-humanizer.md)、[Stop Slop](stop-slop.md)

## Why it made the cut
去 AI 味类的上游原版，SKILL.md + 多 agent 插件清单齐全，规则具体可执行，社区信号极强。
