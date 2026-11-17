# Modern Java Guidance（现代 Java / Spring Boot 护栏）

**Tags:** java, spring-boot, lint, hook, skill
**Source:** [@sivalabs](https://x.com/sivalabs/status/2122834579895763396) · 2026-11-18
**Engagement:** 发现帖 2 赞 / 5 收藏 / 150 次展示；仓库 [wkd09/modern-java-guidance](https://github.com/wkd09/modern-java-guidance) 现 5★，MIT（2026-11-17 建仓）

## When to use
编码 agent 在 Java 17/21/25+ 或 Spring Boot 3.x 项目里仍写出 Java 8 / Spring Boot 2.x 旧模式（`javax.*`、`WebSecurityConfigurerAdapter`、`RestTemplate`、`Executors.newFixedThreadPool()` 等）时；或要扫现有代码找可现代化的写法，同时不能误伤仍停在 Java 8 / Boot 2.x 的仓库。

## What it does
三件套：精简的 Agent Skill（`SKILL.md` 约 4.1 KB）、零第三方依赖的 `mjg` CLI（先探测项目版本再检索/取出 Before/After 指南），以及在每次编辑后扫描 `.java` 文件的 `PostToolUse` 钩子（文档称约 31 ms、不耗模型 token）。规则按检测到的 JDK / Boot 版本门控。仓库对标 [Modern Web Guidance](modern-web-guidance.md)，附 6 项 A/B 评测（引导 + 钩子后 6/6 通过，含一条「不误报遗留项目」）。

## Recipe / links
- Repo: https://github.com/wkd09/modern-java-guidance（MIT，5★）
- 一键安装 CLI + Skill + Hook：`curl -fsSL https://raw.githubusercontent.com/wkd09/modern-java-guidance/main/install.sh | bash`，然后 `mjg setup --target all --dir /path/to/your/spring-boot-project`
- 或：`npx skills add wkd09/modern-java-guidance`；`gh skill install wkd09/modern-java-guidance`
- 试用（不安装）：`uvx --from git+https://github.com/wkd09/modern-java-guidance.git mjg search "security"` / `retrieve BOOT-002` / `check .`

## Why it made the cut
场景清楚，有可运行的 CLI、钩子、SKILL.md 和 CI 评测，定位是已收录官方包 Modern Web Guidance 的 Java/Spring 对应物。仓很新、星标很少，安装前需自审；后续看规则覆盖是否继续增长。
