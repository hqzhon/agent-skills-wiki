# CLI-Anything（把任意软件变成 Agent 可调用的 CLI）

**Tags:** cli, agent-native, tooling, skill-pack, official-lab
**Source:** [@Aw5295388256244](https://x.com/Aw5295388256244/status/2123229067294253299) · 2026-11-19
**Engagement:** 今日 GitHub 热榜相关转述帖；仓库 [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) 约 59,962★，Apache-2.0（港大 HKUDS，技术报告 arXiv:2606.03854）。本轮才写入目录。

## When to use
希望编码 agent（Claude Code、Codex、Cursor、OpenClaw 等）像用人类 CLI 一样操作 GIMP、Blender、Obsidian、LibreOffice 等桌面或专业软件，或要给尚无 agent 接口的软件自动生成一套命令行 harness + SKILL.md 时使用。

## What it does
两条入口：① **CLI-Hub** 浏览并安装社区已做好的 agent-native CLI（文档称现成 60 多个）；② 用仓库自带的各宿主 skill，跑 7 阶段流水线，为指定软件生成 CLI、schema、测试和 SKILL.md。仓库内有多份宿主 skill（如 `codex-skill`、`hermes-skill`、`cli-hub-meta-skill` 等），README 称 2,461 项测试通过，覆盖约 11 个 agent 平台。生成的命令面向 agent：结构化 JSON 输出，而不是只给人看的交互界面。

## Recipe / links
- Repo: https://github.com/HKUDS/CLI-Anything（Apache-2.0，约 59,962★）
- 文档 / Hub: https://clianything.cc/ · https://hkuds.github.io/CLI-Anything/
- 先用现成 CLI：
  ```bash
  pip install cli-anything-hub
  cli-hub list
  cli-hub search image
  cli-hub install gimp
  cli-hub launch gimp
  ```
  部分 CLI 依赖本机已安装对应软件。
- 给自己的 agent 装生成器 skill（按宿主选 skill 名）：
  ```bash
  npx skills add HKUDS/CLI-Anything --skill <skill-name> -g -y
  ```

## Why it made the cut
把「让 agent 用上现有软件」落成可安装的 CLI 生态和可复现的 skill 生成流水线，而不是再包一层演示脚本；社区信号与测试规模都很高。注意：这是工具链 + skill 包，不是单一任务配方。
