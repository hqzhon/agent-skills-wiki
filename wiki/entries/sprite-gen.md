# sprite-gen（一张立绘做成游戏精灵表或透明循环动画）

**Tags:** gamedev, sprites, animation, atlas, cli, skill
**Source:** [@dextune](https://x.com/dextune/status/2125970017896501568) · 2026-11-26
**Engagement:** 介绍帖 134 赞 / 147 收藏 / 17 转（本窗宣布 v4.4.0）；仓库 [aldegad/sprite-gen](https://github.com/aldegad/sprite-gen) 现 4,306★，Apache-2.0。2026-05-12 创建，本窗仍有推送。

## When to use
你有一张角色静帧，想得到引擎能用的精灵表（带透明度和 manifest.json.frame_layout），或一段抠好背景的循环动画时用。不要指望直接让图像模型「出一张 sprite sheet」——作者写明那种结果通常对不齐、抠不干净、也不能直接进引擎。与已收录的 [sprite-stacking](sprite-stacking.md)（四视图叠成伪 3D）和 [spritecast](spritecast.md)（按镜头角度出 8 向图）不是同一条路。

## What it does
以 Codex / Claude skill + Python CLI 的形式，按状态行驱动出图、锁住角色身份、把色键背景收成真 alpha、提取帧并合成运行时 atlas；也可以把同一张静帧交给视频模型，再修跳跃帧、统一循环长度。v4.4.0 调整了出图/朝向检查所用模型，并恢复 Python 3.11 兼容、升级到 Pillow 13。出图走你自己的 Codex / Grok /（可选）OpenAI 凭据，仓库不附带密钥；需要 API key 的调用会在请求前打到 stderr。需要 CPython 3.11+（CI 跑 3.14），并在 venv 里安装。

## Recipe / links
- Repo: https://github.com/aldegad/sprite-gen（4,306★，Apache-2.0）
- 作为 skill 安装（仓库 README）：
  ```bash
  python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py --repo aldegad/sprite-gen --path . --name sprite-gen
  ```
- CLI：
  ```bash
  python3 -m venv .venv && source .venv/bin/activate
  pip install -e .
  sprite-gen --help
  ```
  atlas 流程：prepare → gen-set → extract → compose-atlas（可选 curation）。视频循环流程：sprite-gen video-set ...（需 ffmpeg、img2webp，以及已登录的 grok 或 XAI_API_KEY）。

## Why it made the cut
可加载 skill + 完整 CLI 流水线，场景和「不要直接要一张 sprite sheet」的边界都很清楚；4.3k★，本窗介绍帖互动也高。
