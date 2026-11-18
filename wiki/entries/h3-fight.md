# h3-fight（MiniMax H3 打戏提示词）

**Tags:** video, prompt-writing, minimax, motion, skill
**Source:** [@ShenfuX](https://x.com/ShenfuX/status/2122948653908373645) · 2026-11-18
**Engagement:** 发现帖为讨论向回复（1 赞 / 25 次展示）；仓库 [huangserva/h3-fight](https://github.com/huangserva/h3-fight) 现 133★（2026-11-15 建仓，仍在推送）。`工具/` 代码 MIT，提示词库与演示 GIF 为 CC BY-NC 4.0

## When to use
用 MiniMax H3 写武打、刀剑、弓箭、徒手、气功对波、追逐、以小打大、团战，或滑雪/滑板/跑酷等大动作运动的提示词，要把剧本里的打斗或运动节拍变成镜头，而不想每次从零手写。不适合文戏，也不适合以闪电/法术特效为主的镜头。与官方 [h3-image-prompt-writing](minimax-h3-image-prompt-writing.md)（偏出图提示词）互补。

## What it does
从出过好片的提示词库里挑镜头块，整句搬、只换名词，再跑提交前检查，然后出片、看片、把新经验写回库。库里有镜头块、词句零件、招式表和踩坑表；运动题材先看 `运动.md`，广告片后期（放大、配乐对点、旁白、品牌结尾）看 `广告后期.md`。可选 ComfyUI 出片。检查脚本会卡朝向、防越轴、防人物「回到定妆图站姿」。

## Recipe / links
- Repo: https://github.com/huangserva/h3-fight
- 安装：
  - Claude Code：`git clone https://github.com/huangserva/h3-fight.git ~/.claude/skills/h3-fight`
  - Codex：`git clone https://github.com/huangserva/h3-fight.git ~/.codex/skills/h3-fight`
- 然后在技能目录执行 `pip install -r requirements.txt` 和 `python3 工具/自检.py`；出片后的拼图/字幕还需要 ffmpeg。重开会话后才会被识别。Windows 需注意中文路径（`core.quotepath false` + UTF-8 终端）。
- 提示词库为 CC BY-NC 4.0，商业使用前先读 `库/LICENSE.md`。

## Why it made the cut
场景很窄但配方完整：有库、检查脚本和可核对的防反规则，不是一份「把打戏写得好看」的空提示。许可要分开看。
