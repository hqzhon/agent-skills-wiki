# jevgrep（用自然语言问仓库「这段行为在哪」）

**Tags:** code-search, cli, discovery, semantic-search, skill
**Source:** [@hsianghui](https://x.com/hsianghui/status/2126055353871917208) · 2026-11-27
**Engagement:** 介绍帖 6 赞 / 5 收藏；仓库 [dzhng/jevgrep](https://github.com/dzhng/jevgrep) 现 3,271★，MIT。需 Node.js 22+，最近推送到 2026-11-12。

## When to use
面对不熟悉的代码库，要问「遥测是怎么发出去的」「认证在哪一道检查」这类**行为 / 生命周期**问题，并希望先拿到相关文件和原文摘录再动手改时用。精确符号、字符串或文件名查找仍用 grep / 文件搜索；不要把 jg 当成通用关键词搜索。

## What it does
CLI `jg` 用 [Jev](https://vercel.com/ai-gateway/models/jev) 在目录、文件和声明之间判断相关性，一次标准输出返回相关文件、阅读线索和源代码摘录。仓库强调：**只装 CLI 不会让编码 agent 会用它**，还要用 `jg skill` 安装配套 skill。作者在十项 SWE-bench 对照里写到：与基线同样完成 8/10，成本更低。需要 Vercel AI Gateway、TypeSafe、OpenRouter、OpenCode Zen 或兼容端点的密钥；`jg auth` 是交互式登录，技能要求不要在对话里索要 API key。

## Recipe / links
- Repo: https://github.com/dzhng/jevgrep（3,271★，MIT）
- npm: https://www.npmjs.com/package/@dzhng/jevgrep
- 技能：https://github.com/dzhng/jevgrep/blob/main/skills/jevgrep/SKILL.md
- 安装：
  ```bash
  npm install -g @dzhng/jevgrep
  jg auth
  jg skill
  jg "How are telemetry events recorded and sent?" ./my-project
  ```

## Why it made the cut
可加载 skill + 可独立运行的 CLI，场景写得很清楚（行为发现，不是再做一个 grep）；有安装步骤、鉴权边界和对照实验说明，社区信号也足够。
