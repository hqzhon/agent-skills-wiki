# Joggernaut（找出 GitHub Actions 上 PR 在等什么）

**Tags:** ci, github-actions, performance, diagnostics, skill-pack
**Source:** [@ai_algoit](https://x.com/ai_algoit/status/2125438246226366950) · 2026-11-25
**Engagement:** 本窗介绍帖 1 赞；仓库 [usejog/joggernaut](https://github.com/usejog/joggernaut) 现 60★，MIT，2026-11-25 仍在推送

## When to use
PR 卡在 GitHub Actions 上、说不清时间花在排队、安装还是测试时用。技能会读你自己的 run 记录做诊断，选中修复方案后才改仓库文件；合并后可以再测一次修复是否真的缩短了等待。作者声明尚未在别人的 CI 上做过系统测量。

## What it does
7 个技能：`ci-diagnose`（默认每个 workflow 读约 150 次 run，把等待拆成排队 / 安装 / 运行并按耗时排序）、`ci-measure`（对比修复前后，并用 CI 保存的 JUnit 报告按名字核对测试仍都跑了）、以及 cache、workflow、slow tests、flaky tests、guard。规则包括：未得到确认前不改被跟踪文件；一次 PR 只做一件改动；不删测试。只通过本机已登录的 `gh` 发 GET 请求读 run。

## Recipe / links
- Repo: https://github.com/usejog/joggernaut（60★，MIT）
- Claude Code：`/plugin marketplace add usejog/joggernaut` → `/plugin install jog@joggernaut`，然后 `/reload-plugins`
- 其他宿主（需 Node.js 22.20+）：`npx skills add usejog/joggernaut -g -y -a codex`（把 `codex` 换成 cursor / opencode 等）
- 依赖：仓库使用 GitHub Actions、Python 3.9+、已 `gh auth login` 的 GitHub CLI
- 注意：`npx skills` 默认会发送安装遥测，可按该 CLI 的说明关闭

## Why it made the cut
配方非常具体：诊断 → 你点头再改 → 用前后 run 和 JUnit 验收，有 7 个可加载 SKILL.md。星数一般，但场景和验证步骤清楚，不是空喊「加速 CI」。
