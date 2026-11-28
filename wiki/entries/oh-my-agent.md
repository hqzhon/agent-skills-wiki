# oh-my-agent（按任务装技能，或拉起规划-开发-审查团队）

**Tags:** workflow, multi-agent, review, hooks, skill-pack
**Source:** [@cheery9998](https://x.com/cheery9998/status/2126527502986485827) · 2026-11-28
**Engagement:** 本窗来自一篇 Antigravity 工具盘点（13 赞 / 10 书签），不是作者第一方；仓库 [first-fluke/oh-my-agent](https://github.com/first-fluke/oh-my-agent) 1,481★，MIT。同一帖里另外两个是界面插件（agy-beautify、antigravity-session-preview），不按技能收录。

## When to use
想在已有的 Claude Code / Codex / Cursor 等环境里**先装一个任务技能**（审 AI 写的代码、看后台页层级、复现失败测试、看系统边界），或者把代理变成「规划 → 并行开发 → 审查 → 调试」的小团队时用。只想要一条治理规则文件、不要技能包时，不必装整套；同窗出现的 [agentic-os](https://github.com/KbWen/agentic-os) 更偏 AGENTS.md 门禁，本窗未单列，继续观察。

## What it does
可加载的技能与领域预设，也可安装完整 `oma` 工作流（hooks、并行门和测试门）。README 给的单技能入口包括：
- `oma-qa`：审查 diff，指出缺陷并引用行号
- `oma-design`：看管理后台的层级和表格密度
- `oma-debug`：复现失败测试、修根因并跑相关检查
- `oma-architecture`：审查 API 与 worker 等边界
- 完整安装后可用 `/oma-mode` 把任务交给整队

文档里有给代理看的非交互安装指南。面向 Claude Code、Codex、Cursor 等十多种编码代理。

## Recipe / links
- Repo: https://github.com/first-fluke/oh-my-agent（1,481★，MIT）
- 装单个技能（在当前项目）：
  ```bash
  bunx skills use first-fluke/oh-my-agent@oma-qa
  ```
- 完整安装：
  ```bash
  curl -fsSL https://raw.githubusercontent.com/first-fluke/oh-my-agent/main/cli/install.sh | bash
  ```
  或让代理阅读 https://raw.githubusercontent.com/first-fluke/oh-my-agent/main/docs/agent-install.md 后自行安装。
- 站点：https://firstfluke.com/oh-my-agent/

## Why it made the cut
星数和许可都过线，技能可按任务单独装，也有完整团队工作流；本窗来源是盘点帖，不是第一方发布，条目里标明。不要和同帖的主题皮肤、会话预览插件混成一条。
