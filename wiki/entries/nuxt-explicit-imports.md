# nuxt-explicit-imports（Nuxt 自动导入 → 显式导入）

**Tags:** nuxt, migration, codemod, typescript, frontend, skill
**Source:** [@aidevbird](https://x.com/aidevbird/status/2122505086681403606) · 2026-11-17
**Engagement:** 发现帖互动很低；仓库 [antfu/nuxt-explicit-imports](https://github.com/antfu/nuxt-explicit-imports) 新建于 2026-11-16，现 6★，MIT；作者 Anthony Fu

## When to use
要把 Nuxt 4 应用从 auto-imports 迁到显式 import：准备关闭自动导入、看到 `[nuxt-explicit-imports]` 警告或 strict 模式构建失败，或正在配置 `explicitImports`。不适合仍打算长期依赖自动导入、只想改几个文件的场景。

## What it does
模块 + agent skill + codemod。按三个可独立推进的类别迁移：`imports`（Vue/Nuxt composables、`composables/`、`utils/`）、`components`（模板组件与 `Lazy*`）、`server`（Nitro / `server/`）。每类按 `warn → 迁移并自检 → strict` 单向棘轮前进：`check` 列出隐式使用，`migrate` 写入可自动修复的 import，手工项见 `references/manual-fixes.md`。skill 要求先记录 typcheck / lint / test / build 基线，按目录小步迁移，每步对照基线，再把该类别打成 strict。

## Recipe / links
- Repo: https://github.com/antfu/nuxt-explicit-imports （MIT）
- SKILL.md: `skills/nuxt-explicit-imports/SKILL.md`
- 安装：
  ```bash
  npx nuxi module add nuxt-explicit-imports
  npx skills add antfu/nuxt-explicit-imports
  ```
  然后让 agent：「用 nuxt-explicit-imports skill 把本应用迁到显式导入。」

## Why it made the cut
完整、可执行的 `SKILL.md`：场景、步骤、验收和陷阱写得很清楚，并配有可自检的 CLI。仓库还很新、星标很少，但作者与配方质量够格收录；后续以仓内维护为准。
