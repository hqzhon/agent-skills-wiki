# generate-icons（先出样再画完整图标库）

**Tags:** icons, design-system, svg, frontend, react, skill
**Source:** [@ChrisL_AI1022](https://x.com/ChrisL_AI1022/status/2126360405161418872) · 2026-11-27
**Engagement:** 本窗为说明帖（1 赞），非作者第一方；仓库 [sergiobanhos/generate-icons](https://github.com/sergiobanhos/generate-icons) 现 173★ / 12 forks，MIT。此前出现在盘点帖观察名单，本窗有了可核的专用介绍。

## When to use
要一套**匹配现有设计系统**的原创图标库，而不是直接从通用图标集里挑，或让模型一次画完再返工时用。技能会先读项目的 token、主题、字体和已有图标，归纳网格、描边/填充、圆角和色板，先在真实 UI 里出示 6–8 个样例等你确认，再画完整集合。

## What it does
根目录 [SKILL.md](https://github.com/sergiobanhos/generate-icons/blob/main/SKILL.md) 约定：样例通过后再手写 SVG，并导出 React / Vue / Svelte / React Native 或纯 SVG 组件、sprite、可预览目录和 README，再做校验。适合替换占位 emoji、补产品状态/空状态/导航图标，或统一已有图标风格。

## Recipe / links
- Repo: https://github.com/sergiobanhos/generate-icons（173★，MIT）
- 安装：
  ```bash
  npx skills add sergiobanhos/generate-icons
  ```
- 仓库含 `docs/`、`examples/` 与参考资料，可先看样例再跑全库。

## Why it made the cut
「先出样、等人点头再全量生成」写进了配方，使用场景清楚，有 SKILL.md 和 MIT 许可。上轮只在盘点帖里出现，本窗有了可独立阅读的介绍，且星标已到 173，达到单列标准。
