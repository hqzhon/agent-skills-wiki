# Form & Force（先定方向，再按栈实现并对照渲染结果评判）

**Tags:** design, frontend, motion, ui, ux, claude-code, skill
**Source:** [@erendeveloper0](https://x.com/erendeveloper0/status/2125672967124525437) · 2026-11-26
**Engagement:** 本窗为作者征求实测的帖（1 赞）；仓库 [erenthedeveloper0/form-and-force](https://github.com/erenthedeveloper0/form-and-force) 现 5★ / 1 fork，MIT，带 CI；README 标明 pre-1.0，模型评测尚未跑过

## When to use
要让编码 agent 给现有页面做有方向的界面/动效设计：先选定不同于默认模板的创意方向，再在你的技术栈里实现，并用浏览器渲染结果去对照「一个普通 agent 会做出的平均解」。适合「定价页看起来像所有 SaaS 模板，请按真用户比较套餐的方式重设计，并保留 Next.js」这类任务。它不是只删 AI 痕迹的清洁工（那是 [unslop-ui](unslop-ui.md)），也还不是已经用评测证明「一定更好」的成品。

## What it does
一份可移植 Agent Skill（`skills/form-and-force/SKILL.md`）和 Claude Code 插件。安装后用自然语言描述工作即可；技能会在动手画之前先给出方向，再构建，再判断渲染页。仓库带 `docs/`、`evals/`、`tests/` 和 Playwright/Chromium 工具说明（Chromium 装在项目或缓存目录，不装到全局）。作者写明：方法和工具是完整且经过测试的，但「技能是否提高 agent 产出」的模型评测尚未在任何版本上跑过；Claude Code 插件安装已在 2.1.322 / 2.1.325 上验证。无遥测。

## Recipe / links
- Repo: https://github.com/erenthedeveloper0/form-and-force（5★，MIT）
- SKILL.md：https://github.com/erenthedeveloper0/form-and-force/blob/main/skills/form-and-force/SKILL.md
- 安装（Claude Code）：
  ```bash
  claude plugin marketplace add erenthedeveloper0/form-and-force
  claude plugin install form-and-force@form-and-force
  ```
- 本地试跑：`claude --plugin-dir ./form-and-force`
- 文档：https://github.com/erenthedeveloper0/form-and-force/blob/main/docs/README.md

## Why it made the cut
有可加载 SKILL.md、插件安装路径、文档和 CI，使用场景比「把页面做漂亮」更具体（方向 → 按栈实现 → 对着渲染结果评判）。星数和帖子互动都很低，且作者主动标明评测未跑，按完整配方收录，同时保留 pre-1.0 限制。
