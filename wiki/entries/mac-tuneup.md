# mac-tuneup（先测量再安全清理 Mac）

**Tags:** macos, diagnostics, storage, icloud, skill
**Source:** [@sencanon](https://x.com/sencanon/status/2123043472869396884) · 2026-11-18
**Engagement:** 作者本人介绍帖（0 赞）；仓库 [osencan/mac-tuneup](https://github.com/osencan/mac-tuneup) 为 2026-11-18 新建、1★，MIT（早期条目）

## When to use
Mac 变慢、启动盘或 iCloud 快满，或想做一次安全清理时。技能强调先测量、再让用户自己跑修复脚本。

## What it does
只读诊断脚本先查明原因（健康、空间去向、iCloud 占用、下载失败等），再按模板给出用户可运行的修复脚本；另有一套经验证后再删除的 iCloud 照片外置盘迁移（按文件名和精确大小核对）。三条真实案例说明主因可能完全不同（Fusion Drive 与崩溃守护进程、内存被打开的应用占满、磁盘被模拟器和缓存填满），所以禁止未测量先动手。明确不关安全更新 / Spotlight / Gatekeeper / SIP / FileVault，也不格式化磁盘；删除数据默认进废纸篓并带时间戳。

## Recipe / links
- Repo: https://github.com/osencan/mac-tuneup（MIT，1★）
- Claude Code：`cp -r mac-tuneup ~/.claude/skills/`（技能在仓库的 `mac-tuneup/` 子目录）
- Claude 应用：把该文件夹打成 zip 后在 Settings > Capabilities > Skills 上传
- 关键文件：`mac-tuneup/SKILL.md`，`scripts/diagnose.sh` 等只读脚本，`references/pitfalls.md` 与 `fix-patterns.md`

## Why it made the cut
有明确的安全边界和可运行的只读脚本，不是「让 agent 随便清一下电脑」；案例和陷阱说明来自实际调优。仓很新，属早期收录。
