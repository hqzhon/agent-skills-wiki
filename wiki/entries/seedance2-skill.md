# Seedance 2.0 Prompt Skill（即梦视频提示词）

**Tags:** video, prompt, seedance, jimeng, bytedance, skill
**Source:** [@Chenfacai0](https://x.com/Chenfacai0/status/2125904397226119468) · 2026-11-26
**Engagement:** 本窗中文介绍帖 3 赞；仓库 [dexhunter/seedance2-skill](https://github.com/dexhunter/seedance2-skill) 现 4,584★，MIT。中英两份 `SKILL.md`，内容整理自字节官方手册与案例；仓最近推送停在 2026-09-19。

## When to use
要用即梦 **Seedance 2.0** 做多模态视频、手上已有图/视频/音频素材，但提示词写不清 `@` 引用角色、运镜或场景类型时用。它帮你写提示词，不代替即梦出片，也不适用于其他视频模型的提示词规范。

## What it does
把官方约束做成可加载指南：输入上限（图 ≤9、视频 ≤3、音频 ≤3、合计 ≤12）、输出时长与分辨率、不能上传写实人脸等限制；核心是 `@Image1` / `@Video1` / `@Audio1` 的角色标注（首帧、运镜参考、听感等）。另有运镜和景别词表，以及人物一致性、视频延长、音乐卡点、一镜到底、电商展示、短剧等场景写法和 6 个现成模板（产品广告、短剧、舞蹈、风光卡点、仙侠、科普动画）。

## Recipe / links
- Repo: https://github.com/dexhunter/seedance2-skill（4,584★，MIT）
- 英文：https://github.com/dexhunter/seedance2-skill/blob/main/SKILL.md
- 中文：https://github.com/dexhunter/seedance2-skill/blob/main/zh/SKILL.md
- 安装：
  ```bash
  npx skills add dexhunter/seedance2-skill
  # 或手动复制：
  cp SKILL.md ~/.claude/skills/seedance-prompt-en.md
  cp zh/SKILL.md ~/.claude/skills/seedance-prompt-zh.md
  ```
- 官方来源（飞书文档）：[使用手册](https://bytedance.larkoffice.com/wiki/A5RHwWhoBiOnjukIIw6cu5ybnXQ)、[实战案例](https://bytedance.larkoffice.com/wiki/LJXzwehluiFdzKkb1recZdfonZg)

## Why it made the cut
场景清楚、中英 `SKILL.md` 可装，并写明输入限制与 `@` 引用语法；4,584★、MIT，是本窗漏收的高星技能包。注意仓已约两个月没有新推送，即梦产品若改规则需自行对照官方文档。
