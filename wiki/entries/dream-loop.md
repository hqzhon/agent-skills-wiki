# dream-loop（目标截图闭环做高保真画面）

**Tags:** 3d, games, visuals, image-generation, blender, critic, skill
**Source:** [@Yashpatil](https://x.com/Yashpatil/status/2121448245427675383) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [achimala/dream-loop](https://github.com/achimala/dream-loop) 约 2.1k★（帖中称约 26 小时 +126），207 forks，MIT

## When to use
要 agent 做一个「画面必须好看」的游戏、应用或 3D 场景，且你希望它先锁定一张目标截图，再对着截图迭代，而不是口头描述后一次性交稿。作者示例包括等距、体素风、可在浏览器里跑的 Three.js 演示。

## What it does
一条完整 SKILL.md：先用图像生成「梦」出目标截图（或使用你提供的图）存为 `.dream-loop/target.png`，再按目标去搭建；单独的 critic 子 agent 对比实机截图与目标并给反馈，循环直到满意，可选地再梦一个更高目标。Plus / Pro 两套互不兼容的工作流，按订阅档位只读其中一份。需要图像生成（内置或 API）和视觉输入，子 agent 强烈建议；做自定义 3D 时建议装 Blender（MCP 或脚本优于电脑操控）。目前主要在 Codex 上验证。工作文件放在应被 gitignore 的 `.dream-loop/`。

## Recipe / links
- Repo: https://github.com/achimala/dream-loop
- SKILL.md: https://github.com/achimala/dream-loop/blob/main/SKILL.md
- 安装：`npx skills add achimala/dream-loop`
- 示例演示：https://dream-loop-demo.anshu.dev
- 作者：[@anshuc](https://x.com/anshuc)
- 没有图像生成工具时，skill 会停下来请你提供目标图或接上生图 API

## Why it made the cut
可执行闭环很清楚（目标图 → 搭建 → critic → 再迭代），有 SKILL.md、工作流参考和可点开的演示；仓库星标和 forks 足以验证，不是只靠口头「让 AI 把画面做好看」。
