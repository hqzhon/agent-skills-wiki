# spritecast（按镜头角度出游戏精灵图）

**Tags:** gamedev, sprites, pixel-art, claude-code, skill
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2123016010366144917) · 2026-11-18
**Engagement:** 与 rust-anything 等一并出现在发现帖（约 4 赞 / 277 次展示）；仓库 [Sunghwan0112/spritecast](https://github.com/Sunghwan0112/spritecast) 现 288★，MIT（2026-11-03 建仓，仍在推送）

## When to use
要为等距或其他固定镜头的游戏，从一张角色立绘生成能走路的精灵图：8 向行走、更多动作、像素画、坐姿，或按角色比例出道具。需要每一帧都是同一个人、同一机位，而不是各画各的。

## What it does
Claude Code 插件：身体、动作、角度和阴影由 3D 决定，画面由图像模型绘制。可出 8 向行走、跑跳砍投等动作（或从 Mixamo FBX 来）、约 100px 高的像素表、四足动物行走，以及让角色坐到你自己的道具上。也可以把绘制面数降到 4 个对角方向以节省费用。第一次运行会用 `doctor.py --fix` 在 `~/.cache/spritecast/` 建独立 venv，不改你的系统 Python。依赖 Python 3.9+ 和 Chrome/Edge。

## Recipe / links
- Repo: https://github.com/Sunghwan0112/spritecast（MIT，288★）
- 安装：`claude plugin marketplace add Sunghwan0112/spritecast`，再 `claude plugin install spritecast@spritecast`（或在 Claude Code 里 `/plugin marketplace add Sunghwan0112/spritecast` → `/plugin install spritecast@spritecast`）
- 想免费试用可让 Claude「try SpriteCast」。正式出图需你自己的 OpenAI 与 Tripo 额度；付费步骤会先报价再等确认。
- Skill 路径：`skills/spritecast/SKILL.md`

## Why it made the cut
场景具体，有完整插件/SKILL.md、参考文档和本地脚本，不是一张提示词。需注意它会调用付费图像/3D API。
