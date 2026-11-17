# Zazzy Skills（animate-my-work：Figma → 动效成片）

**Tags:** motion, figma, remotion, animation, skill-pack
**Source:** [@zazzygfx](https://x.com/zazzygfx/status/2122680715393241336) · 2026-11-17
**Engagement:** 发现帖 60 赞 / 4 转帖 / 41 收藏 / 1360 次展示；仓库 [zazzygfx/skills](https://github.com/zazzygfx/skills) 现 2★，MIT（音效/配乐文件另行保留；2026-11-16 建仓）

## When to use
要把 Figma 画板（或 Krea / FLORA / 品牌图）做成有分镜、踩点剪辑和能听清的音效的成品动效片，而不是硬切 + 整屏跟着节拍弹的「幻灯片」。也可先让 `ask-zazzy` 指路该调用哪条 skill。

## What it does
当前可装的技能主要是 `animate-my-work`：收集 brief → 可选参考片分析 → 写 `SCRIPT.md` 节拍表 → 在 Figma 里分镜 → 导出图层 → 用 Remotion 模板渲染，并可按小节线重剪配乐、混合音效。支持一气呵成、逐步确认、只出分镜，或把画板做成循环 GIF。包里另有 `ask-zazzy` 做技能分诊。仓库说明 Remotion 对个人和不超过 3 人的公司免费，更大的公司需要 Remotion 公司许可；`animate-my-work` 的模板基于 design.how 的 make-motion（MIT）。

## Recipe / links
- Repo: https://github.com/zazzygfx/skills（MIT，2★；`skills/animate-my-work/template/public/sfx` 与 `public/music` 不在 MIT 范围内）
- 安装：`npx skills@latest add zazzygfx/skills`
- Claude Code：`/plugin marketplace add zazzygfx/skills` → `/plugin install zazzy-motion@zazzy-skills`
- 调用示例：`/animate-my-work <brief>`；逐步模式用 `/animate-my-work step <brief>`

## Why it made the cut
配方具体（分镜 → 导出 → Remotion 渲染 → 踩点与混音），有 SKILL.md 和标准安装方式，原帖互动不错。仓很新、星标很少；商用前需同时核对 Remotion 许可和音效/配乐版权。
