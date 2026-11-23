# sprite-stacking（四视图像素画叠成可旋转伪 3D 精灵）

**Tags:** gamedev, pixel-art, sprites, fake-3d, skill
**Source:** [@dwhitedesign](https://x.com/dwhitedesign/status/2123815052553650499) · 2026-11-21
**Engagement:** 作者发布帖 918 赞 / 84 转 / 1080 收藏；仓库 [danielwh2/sprite-stacking](https://github.com/danielwh2/sprite-stacking) 450★，MIT。本窗新建（2026-11-20）。

## When to use
想把一张 **上 / 侧 / 前 / 后** 四视图像素稿，做成可以旋转展示的伪 3D 精灵（转盘、Godot 素材等），并且让 Claude Code、Codex、Cursor 等 agent 直接出图和切片时使用。它和已收录的 [spritecast](spritecast.md)（按镜头角度从立绘出 8 向精灵图）不是同一件事。

## What it does
可装 agent skill，附 Python / Pillow / NumPy 切片脚本。流程是：

1. **Views：** 正交的顶、侧、前、后，排成一行
2. **Carve：** 只有四个视图都覆盖到的体素才保留
3. **Slices：** 把体积切成一层层扁平切片（地面在下）
4. **Render：** 每层旋转、按俯仰压扁，再上移 1 像素叠起来

没有现成原图时，agent 可以用短 Python 脚本自己画四视图。仓库还提供 `views_to_slices.py` CLI（层数、预览图、HTML 查看器）。

## Recipe / links
- Repo：https://github.com/danielwh2/sprite-stacking（MIT，450★）
- 安装：
  ```
  npx skills add danielwh2/sprite-stacking
  ```
  也可把 `skills/sprite-stacking` 拷进 `~/.claude/skills/` 或 `~/.agents/skills/`。
- 用法示例：「Make a rotatable pixel art car.」「Sprite stack this 4-view sheet and give me a turntable.」

## Why it made the cut
作者原帖给出完整配方和可运行脚本，场景具体，社区信号强；与 spritecast 互补，不是又一个「帮我出精灵图」提示。
