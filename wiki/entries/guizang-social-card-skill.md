# Guizang Social Card Skill（小红书图文 / 公众号封面对）

**Tags:** social, xiaohongshu, wechat, design, html, live-photo, skill
**Source:** [@heyrimsha](https://x.com/heyrimsha/status/2125207339993276815) · 2026-11-24
**Engagement:** 本窗为内容工具盘点帖（79 赞）提到；仓库 [op7418/guizang-social-card-skill](https://github.com/op7418/guizang-social-card-skill) 现 8,249★，AGPL-3.0，2026-10-30 仍有推送

## When to use
要把文章、脚本、截图、产品说明、字幕、照片或视频，做成**小红书/Rednote 图文**（含 3:4 封面、Live Photo 卡片/拼图）或**微信公众号 21:9 + 1:1 封面对**时用。不要用它去改「瑰藏」原版 PPT 技能。

## What it does
根目录可加载 [SKILL.md](https://github.com/op7418/guizang-social-card-skill/blob/main/SKILL.md)（name: `guizang-social-card-skill`）。借用瑰藏 PPT 的视觉原则，但工作流独立：电子杂志风做氛围叙事、瑞士风做事实结构，28 种版式、10 套主题，单文件 HTML 再导出 PNG。也覆盖实况照片、二宫格/三连/四宫格拼图，以及长视频转 Live Photo。

## Recipe / links
- Repo: https://github.com/op7418/guizang-social-card-skill（8,249★，AGPL-3.0）
- 安装：
```bash
npx skills add https://github.com/op7418/guizang-social-card-skill --skill guizang-social-card-skill
```
  也可把仓库克隆到 `~/.claude/skills/guizang-social-card-skill`，确认 `SKILL.md`、`assets/`、`references/` 在场。更新用该目录里 `git pull`。
- 示例：「帮我基于这篇文章做一套瑞士风小红书图文，5 张，IKB 蓝。」导出依赖 Playwright 等本机能力，装前先看 README 的环境说明。
- 许可是 AGPL-3.0，再分发或网络提供时需注意义务。

## Why it made the cut
高星漏收：完整 SKILL.md、场景非常具体（小红书图文 + 公众号封面对），8,249★。本窗只出现在盘点帖里，按仓库信号补上。和已收录的 gzh-design-skill（Markdown→公众号 HTML）互补：这边出的是图片卡片/封面，不是可粘贴 HTML。
