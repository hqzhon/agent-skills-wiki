# Content Skills（选题到发布的短视频与社媒技能包）

**Tags:** video, social, content, short-form, skill-pack
**Source:** [@Duiady](https://x.com/Duiady/status/2126539153622143019) · 2026-11-28
**Engagement:** 本窗介绍帖 4 赞，非作者第一方；仓库 [blotato/contentskills](https://github.com/blotato/contentskills) 213★，AGPL-3.0。这是 Blotato 产品旁的开源技能包，本地有审核看板（默认 http://localhost:4600/dashboard/）。

## When to use
要用编码代理写短视频脚本、做或改竖屏成片、套主题特效、发社媒或做私信跟进时用。许可是 AGPL-3.0（强 copyleft），商用或闭源分发前先看清楚。发帖、花费和成片前，技能要求先停下来等人批准。

## What it does
一套可加载技能，把「选题 → 脚本 → 成片 → 审核 → 发布」拆开，仓库里可见的技能包括 `make-video`、`post-writer`、`viral-hooks`、`repurpose`、`post-scheduler`、`post-grader`、`content-coach`、`brand-brief`、`quality-check`、`generate`、`setup` 等。典型用法：先出分镜页，人在看板上按「Make my video」批准，再按场景批注修改。也可作为 Claude Code 插件从 marketplace 安装。

本窗介绍帖带一点目录式口吻，但上游 README 和 `skills/make-video/SKILL.md` 是可核的工作手册，不是空喊。

## Recipe / links
- Repo: https://github.com/blotato/contentskills（213★，AGPL-3.0）
- 安装（README 建议直接对代理说）：
  ```text
  setup https://github.com/blotato/contentskills
  ```
- 或作为 Claude Code 插件：
  ```text
  /plugin marketplace add blotato/contentskills
  /plugin install contentskills --marketplace blotato/contentskills
  ```
- 技能目录：`skills/`（例如 `skills/make-video/SKILL.md`）

## Why it made the cut
有明确使用场景和可加载 SKILL.md，仓库能核对技能拆分和审核门。社区信号中等；介绍不是第一方，且许可更严，条目里如实写出。
