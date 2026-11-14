# skill-sync（一份源，软链到所有 Agent）

**Tags:** skill-infra, sync, cli, multi-agent, symlink
**Source:** [@VanceXin](https://x.com/VanceXin/status/2121487162692739370) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [xinpengfei520/skill-sync](https://github.com/xinpengfei520/skill-sync) 0★，MIT；项目自 2026-07 起维护，当日仍有推送

## When to use
同时用 Claude Code、Codex、Cursor、Gemini CLI、Copilot、Windsurf、WorkBuddy 等多个 agent，skills 分散在不同目录：在一个里装了，别的没有；改了一份，其它副本还是旧的。想把技能收成一份源，并用软链镜像到所有已安装的 agent。

## What it does
这是技能基础设施（CLI），不是一条供 agent 加载的 SKILL.md。它把规范副本放在仓库的 `skills/`（本机默认也可收进 `~/.skill-sync`），再对每个已安装 agent 的 skills 目录做软链（Windows 上必要时用 directory junction）：

- 默认 dry-run，不覆盖真实目录；内容冲突标 CONFLICT，不擅自合并；被替换的副本进 backups
- 只管理已经装在机器上的 agent，不替你新建没用过的工具目录
- `init` 可选要同步哪些 agent；`doctor` 检查数量、SKILL.md 行数、description 长度和掉链
- 可选本机定时同步，默认 git 提交、有远程才推送
- 支持 macOS / Linux / Windows

作者帖中称可覆盖约 18 个 agent。同类思路还有仅 Windows 的 DevilukeZhou/skill-sync，以及偏分类扫描的 kina-cmd/agent-skill-sync；本条收录的是带一键安装和 doctor 的这份。

## Recipe / links
- Repo: https://github.com/xinpengfei520/skill-sync
- macOS / Linux 一键安装：`curl -fsSL https://raw.githubusercontent.com/xinpengfei520/skill-sync/main/install.sh | sh`
- 安装脚本会把工具放在 `~/.skill-sync/tool`，并在 `~/.local/bin` 写 `skill-sync` 启动器
- 中文 README：https://github.com/xinpengfei520/skill-sync/blob/main/README.zh-CN.md

## Why it made the cut
场景非常常见（多 agent 技能漂移），步骤和安全默认值写得清楚，有可验证的仓库和安装脚本。它本身不是一条业务 skill，但和 [APM（Microsoft）](microsoft-apm.md) 一样属于值得单独记录的技能基础设施。
