# SivaLabs Agent Skills（Spring Boot / Modulith / Java 审查包）

**Tags:** java, spring-boot, spring-modulith, code-review, skill-pack
**Source:** [@sivalabs](https://x.com/sivalabs/status/2126526099480072314) · 2026-11-28
**Engagement:** 作者第一方，本窗说会改掉一批对较新模型过于啰嗦的 Spring Boot 指引，13 赞 / 10 书签；仓库 [sivaprasadreddy/sivalabs-agent-skills](https://github.com/sivaprasadreddy/sivalabs-agent-skills) 196★，MIT。与已收录的 [Modern Java Guidance](modern-java-guidance.md)（另一仓库的现代 Java / Spring Boot 护栏）互补，不是同一包。

## When to use
要用编码代理写或改 Spring Boot 应用、检查 Spring Modulith 边界、补 jSpecify 空安全、做 Java 代码审查，或批量处理 Renovate PR 时用。作者本窗的观点是：新模型不必再塞一批「显而易见」的指引，技能会往更瘦的方向更新。

## What it does
一组可按需安装的 Java / Spring 技能，README 列出：
- `progen`、`spring-boot`、`spring-modulith-verifier`、`jspecify`、`java-code-review`、`apply-renovate-prs`
- 仓库里还有 `pair-programming`

可用 `npx skills add` 装整包或单个技能，也可用 `install.sh` 装到项目级或用户级的 Claude Code / Codex / Gemini / Cursor 技能目录。

## Recipe / links
- Repo: https://github.com/sivaprasadreddy/sivalabs-agent-skills（196★，MIT）
- 安装：
  ```bash
  npx skills add https://github.com/sivaprasadreddy/sivalabs-agent-skills
  npx skills add https://github.com/sivaprasadreddy/sivalabs-agent-skills --skill spring-boot
  ```
- 或：`curl -fsSL https://raw.githubusercontent.com/sivaprasadreddy/sivalabs-agent-skills/refs/heads/main/install.sh | bash`
- 技能目录：`skills/`

## Why it made the cut
第一方维护的可加载 Spring / Java 技能包，许可清楚，和已有的 Modern Java Guidance 不是同一仓库。本窗不是全新发布，但是作者现身说明更新方向，值得补进目录。
