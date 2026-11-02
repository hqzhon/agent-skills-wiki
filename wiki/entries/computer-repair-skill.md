# Computer Repair Skill（电脑维修 Playbook）

**Tags:** it-support, troubleshooting, windows, macos, linux, chinese
**Source:** [@bkdgiffug](https://x.com/bkdgiffug/status/2116840674020716829) · 2026-11-01
**Engagement:** 88lin/computer-repair-skill ~420★，AGPL-3.0，带 CI 校验

## When to use
电脑出问题想让 Agent 帮忙排查修复：C 盘爆满、卡顿、蓝屏 / 开不了机、没声音、连不上网、流氓软件和弹窗、应用与数据迁移、Time Machine / Homebrew / CUDA 等，覆盖 Windows、macOS、Linux。

## What it does
「先取证、再判断；先计划、再修改」：Agent 先读取系统状态、日志、配置和硬件事实，建立候选原因；诊断只读优先，删除、安装、提权、重启、分区、改服务前先给出影响、回滚和验证方案。64 个专项 Playbook 通过路由索引按需加载；存储清理会逐层下钻并报告实测释放空间。纯 Markdown/YAML，可选 Git 存储审计脚本。

## Recipe / links
- Repo: https://github.com/88lin/computer-repair-skill
- 在线浏览 Playbook：https://repair.88lin.eu.org/#playbooks

## Why it made the cut
场景具体、安全边界设计到位（只读优先 + 变更前回滚方案），按需加载的路由结构也是值得参考的大型 skill 组织方式。README 带较多 API 中转赞助广告，可忽略。
