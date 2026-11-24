# RoboDK Agent Skills（官方：从描述到工位/机器人程序）

**Tags:** official, robotics, robodk, manufacturing, skill-pack
**Source:** [@RoboDKinc](https://x.com/RoboDKinc/status/2124873177167720506) · 2026-11-23
**Engagement:** 本窗为官方 Add-In 竞赛宣传帖（1 赞）· 仓库 [RoboDK/RoboDK-Agent-Skills](https://github.com/RoboDK/RoboDK-Agent-Skills) 现 10★，MIT，厂商官方维护；仓最近推送停在 2026-10-06

## When to use
在已安装 RoboDK 的环境里，用自然语言让 agent 搭工位、写 RoboDK API、生成 ABB / FANUC / KUKA / UR 等控制器程序，或做 Add-In / 工位结构检查，而不是纯手工点选。

## What it does
官方 7 个技能：

- `robodk-shape-builder`：按描述放置桌子、围栏、传送带、导轨、龙门、转台等
- `robodk-api`：编写和移植 RoboDK API 代码
- `robodk-post-processor-builder` / `robodk-driver-builder`：后处理与驱动
- `robodk-real-robot-control`：走向真实机器人
- `robodk-addin`：扩展菜单、工具栏和设置对话框
- `robodk-station-audit`：检查工位结构性错误

需要本机安装 RoboDK，以及能加载 `SKILL.md` 的编码 agent（文档以 Claude Code 为例）。

## Recipe / links
- Repo: https://github.com/RoboDK/RoboDK-Agent-Skills（10★，MIT）
- 一键把全部 skill 链到 `~/.claude/skills/`：
  ```bash
  ./scripts/install.sh          # Windows 用 .\scripts\install.ps1
  ```
- 或只拷其中一个，例如：
  ```bash
  cp -r skills/robodk-post-processor-builder ~/.claude/skills/
  ```

## Why it made the cut
厂商官方技能包，7 个可加载 `SKILL.md`，场景具体（工位、API、后处理、真机）。本窗帖偏竞赛宣传，仓库星数不高且 10 月后暂无推送，但材料可验证，按官方包标准收录，并注明维护窗口。
