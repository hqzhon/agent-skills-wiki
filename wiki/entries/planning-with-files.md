# planning-with-files（把计划写到磁盘，清会话也能接着干）

**Tags:** planning, persistence, context, workflow, skill
**Source:** [@hsianghui](https://x.com/hsianghui/status/2124916631558291626) · 2026-11-23
**Engagement:** 本窗介绍帖 12 赞 / 8 收藏 · 仓库 [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) 现 28,209★，MIT；官方评测声称带 skill 后断言通过率 96.7%（29/30），盲测 3/3 胜出

## When to use
长任务、跨多次 `/clear` 或上下文压缩的编码工作：希望计划、发现和进度落在项目里的 Markdown 文件上，而不是只活在对话窗口里。agent 每轮重新注入这些文件，并用完成门禁判断能否收工。

## What it does
按 Manus 风格把工作状态写到磁盘（`task_plan.md`、`findings.md`、`progress.md` 一类计划文件），崩溃或清空会话后可以从文件恢复。原生插件路线还带生命周期钩子（启动、恢复、clear、压缩后自动恢复当前计划）。技能本身走 Agent Skills 标准，号称覆盖 60+ 种 agent；另有阿拉伯语、德语、西班牙语、简体/繁体中文等变体。

## Recipe / links
- Repo: https://github.com/OthmanAdi/planning-with-files（28,209★，MIT，默认分支 `master`）
- Claude Code 插件（技能 + hooks + 斜杠命令）：
  ```
  /plugin marketplace add OthmanAdi/planning-with-files
  /plugin install planning-with-files@planning-with-files
  ```
- 其他 agent（Agent Skills 标准）：
  ```bash
  npx skills add OthmanAdi/planning-with-files --skill planning-with-files -g
  ```
  中文变体把 `--skill` 换成 `planning-with-files-zh` 或 `planning-with-files-zht`。
- 也可 `npm install planning-with-files` 钉进项目依赖（只带文件，不自动注册 hooks）

## Why it made the cut
28k★、MIT、安装路径清楚，并且把「计划必须落盘、清会话还能续上」做成可验证的技能和插件，而不是一句提示词。本窗介绍帖互动一般，按高星漏收补上。
