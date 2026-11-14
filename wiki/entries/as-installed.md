# as-installed（按已安装版本写 API）

**Tags:** dependencies, api, hallucination, node, python, skill
**Source:** [@codewithrashid](https://x.com/codewithrashid/status/2121507011175334228) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [code-with-rashid/as-installed](https://github.com/code-with-rashid/as-installed) 0★，MIT；有 changelog、evals 和测试

## When to use
agent 要写或改第三方库调用，尤其是刚过 major 的 SDK（AI SDK、MCP、框架升级），或已经出现 `ImportError` / `AttributeError` / `cannot import name` / `is not a function` / `has no exported member`。目标是按项目**实际安装的版本**写，而不是模型训练时记住的 API。不负责帮你选依赖或升版本。

## What it does
可移植 Agent Skill：调用第三方包之前，先从 lockfile、`node_modules` 或 `site-packages` 解析真实版本，读该版本的类型、源码和 changelog；改完后再检查变动文件里的每个 import 和名字是否存在于该版本、是否已废弃。支持 npm / pnpm / yarn / bun 和 Python（pip、uv、Poetry）；Go 与 Cargo 只核版本。Claude Code、Codex、Cursor、Gemini CLI、Copilot 等兼容 Agent Skills 的工具都可用。README 举了 MCP Python SDK 2 改导出路径、AI SDK 7 仍能跑但已废弃之类「响/哑」两类事故。

## Recipe / links
- Repo: https://github.com/code-with-rashid/as-installed
- SKILL.md: https://github.com/code-with-rashid/as-installed/blob/main/skills/as-installed/SKILL.md
- 安装：`npx skills add code-with-rashid/as-installed`
- 许可：MIT；需要 Python 3.8+（有 Node 时还会读未标注类型的 npm 包运行时导出）

## Why it made the cut
问题具体（模型记的是旧 API，项目跑的是 lockfile 里的版本），步骤可执行（先解析版本再对照类型/源码，最后再核 import），有 SKILL.md 和测试/evals。星标尚无，但配方完整，值得收录。
