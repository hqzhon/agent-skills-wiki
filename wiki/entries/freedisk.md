# freedisk（macOS 磁盘审计，扫描不删除）

**Tags:** macos, disk, cli, developer-tools, skill
**Source:** [@cip_spiridon](https://x.com/cip_spiridon/status/2121805924281249995) · 2026-11-15
**Engagement:** 发现帖互动低；仓库 [CiprianSpiridon/free-disk-space](https://github.com/CiprianSpiridon/free-disk-space) 现 1★，MIT，v0.3.0；2026-11-14 仍有提交

## When to use
开发用的 Mac 磁盘被 worktree、`node_modules`、`target`、模拟器或 Docker 稀疏盘占满，想先看清「什么在吃空间」，再由你点名要删的 finding id。扫描本身不会删除任何东西。

## What it does
macOS / APFS 上的 agent-first CLI `freedisk`，附带同名 agent skill。流程是：扫描 → 报告（Markdown / JSON）→ 人点名 id → `freedisk delete <id>`。`--quick` 看卷、目录热点、家目录浅层和 tmp 子目录；`--dev` 加上遗留 worktree 和构建产物；默认 full 再加模拟器等更深的盘点。扫描进度打在 stderr，不要中途杀掉还在 `still walking` 的进程。只有 `freedisk delete` 是变更路径：TTY 下按 id 确认，非 TTY 必须加 `--yes`；超过 24 小时的旧扫描会拒绝删除。git 跟踪路径、进行中的 worktree、系统目录和整份 `$HOME` 等会被拒绝删除。skill 还允许 agent 按扫描建议更新本机 catalog 覆盖层（加路径、禁用某类扫描），这也不等于授权删除。

## Recipe / links
- Repo: https://github.com/CiprianSpiridon/free-disk-space（MIT，macOS / APFS only）
- 安装 CLI：`go install github.com/CiprianSpiridon/free-disk-space/cmd/freedisk@latest`（另有 Homebrew / `npx fspace` 说明，见仓库 `docs/`）
- 写入各本地 coding agent 的 skill：`freedisk skill install`（Claude Code、Codex、Cursor、Grok 等）
- Skill 源文件：仓库 `skills/freedisk/SKILL.md`
- 常用：`freedisk scan --quick --json`，再 `freedisk why`；确认 id 后才 `freedisk delete`

## Why it made the cut
可安装的具体配方，场景清楚（开发机磁盘审计），安全边界写得很硬：扫描不删除、只能按人点名的 id 回收。仓库很新、星数还少，先观察后续维护。
