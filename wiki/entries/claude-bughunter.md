# claude-bughunter（授权漏洞狩猎 / 红队技能包）

**Tags:** security, bug-bounty, red-team, skill-pack, claude-code
**Source:** [@musen9527](https://x.com/musen9527/status/2121760285153513802) · 2026-11-15
**Engagement:** 发现帖互动低；仓库 [elementalsouls/Claude-BugHunter](https://github.com/elementalsouls/Claude-BugHunter) 约 5858★ / 901 forks，MIT；2026-11-14 仍有提交

## When to use
只在**已获授权**的漏洞赏金、红队演练，或明确允许的训练靶场（作者列举了 DVWA、OWASP Juice Shop、Hacker101 等）里，让 Claude Code 按漏洞类别做方法论、分流和报告，而不是临场拼提示词。未授权测试不要用。

## What it does
面向 Claude Code 的技能包（README 现记 83 个 skill、15 条斜杠命令）。结构分四层：思考与方法论（如 `bb-methodology`、`redteam-mindset`）；Web 应用狩猎（一组 `hunt-*` skill，材料来自已公开的 HackerOne 披露报告，按类别组织检测思路与报告习惯）；企业周边与身份/基础设施相关的技能；以及分流验证、证据卫生和交付物。仓库还带 engagement 目录脚手架和 Burp MCP 集成说明。相关 skill 按你描述的测试主题自动加载，不必逐个点名。本条目只记录包的用途和安装方式，不转载具体检测步骤或攻击材料。

## Recipe / links
- Repo: https://github.com/elementalsouls/Claude-BugHunter（~5858★，MIT）
- 推荐以 Claude Code 插件安装：
  ```
  /plugin marketplace add elementalsouls/Claude-BugHunter
  /plugin install claude-bughunter@elementalsouls
  ```
  技能和命令会挂在 `claude-bughunter:` 命名空间下，升级插件即可更新，不必拷进 `~/.claude/`。
- 或不走插件、固定某一克隆：`git clone` 后在 macOS / Linux 跑 `bash scripts/install.sh`（Windows 为 `pwsh ./scripts/install.ps1`），会把 skills 和 commands 拷到 Claude 目录。
- 装前读仓库的 LICENSE、README 和安全/范围说明；只对书面授权范围内的目标使用。

## Why it made the cut
可安装的完整技能包，使用场景清楚，仓库与 83 份 SKILL.md 可验证，社区信号强。和本 wiki 已有的 [appsec-skills](appsec-skills.md)、[xss-audit](xss-audit.md) 互补：后两者偏己方代码审计，这一包面向授权的外部狩猎与报告流程。
