# mcu-skills（单片机/开发板固件技能包）

**Tags:** embedded, firmware, esp32, stm32, skill-pack
**Source:** [@techbrosky](https://x.com/techbrosky/status/2123337428479959175) · 2026-11-19（引用帖指向同一仓库）
**Engagement:** 引用介绍帖；仓库 [alexex1993/mcu-skills](https://github.com/alexex1993/mcu-skills) 29★，MIT。

## When to use
用 Claude Code 或 Codex 给 **STM32、ESP32/ESP8266、RP2040、nRF52、AVR** 等开发板写固件，希望 agent **不要猜引脚、时钟树和烧录路径**，而是按这块板的 datasheet / 原理图级知识工作时使用。

## What it does
按板卡拆分的 Agent Skills：一块板一个 `SKILL.md`，把散落在手册、原理图和踩坑经验里的板级知识收进技能（哪根脚干什么、哪套时钟树能工作、哪个 HAL 调用其实没效果、如何把构建烧到芯片上）。覆盖 WeAct STM32 核心板、各类 ESP32/C3/C6/S3/P4 开发板、NodeMCU、nice!nano 类 nRF52840、Arduino Nano 等。安装脚本可一次装全部，或只装某块板；默认用符号链接，`git pull` 即可更新。

## Recipe / links
- Repo: https://github.com/alexex1993/mcu-skills（MIT，29★）
- 安装（Codex 示例）：
  ```
  git clone https://github.com/alexex1993/mcu-skills.git
  cd mcu-skills
  ./scripts/install.sh --codex --all
  ```
  Windows 用 `.\scripts\install.ps1 --codex --all`。可改成只装一块板（如 `rp2040-pico`），或加 `--copy` 做独立副本。`./scripts/install.sh --list` 会同时列出 Claude 与 Codex 的安装路径；Claude Code 的对应参数见仓库 README。
- 项目级安装可设 `CODEX_SKILLS_DIR` 指向该项目的 `.agents/skills`。

## Why it made the cut
嵌入式场景很少被做成可加载技能包，这里有明确的「何时用」、按板卡落地的 SKILL.md 和可重复的安装脚本，不是一句「帮我写 STM32 代码」。
