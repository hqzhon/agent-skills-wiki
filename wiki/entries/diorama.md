# diorama（可旋转 Three.js 立体模型盒）

**Tags:** 3d, threejs, pixel-art, toon, visualization, skill
**Source:** [@scharssazael](https://x.com/scharssazael/status/2124687253721030965) · 2026-11-23
**Engagement:** 本窗提示帖 0 赞；仓库 [sloemo01/diorama](https://github.com/sloemo01/diorama) 710★ / 65 forks，MIT；skill 版本 v5.7.0

## When to use
要做细节充分、可绕视的 Three.js 立体模型盒（战斗、机械、场景叙事），并先决定三种外观之一（经典像素 / 描边卡通 / 像素+描边），以及模型来自现成库还是自己的几何。叙事场景默认不要教学 UI，除非你明确要求。

## What it does
完整长篇 playbook + 代码套件：构图、角色、动画、取材与搭建都写进根目录 `SKILL.md`，并带 `references/`、`templates/`、`verify/` 和示范场景。安装脚本会先问目标目录，再复制约 155 个文件（约 1.6 MB），不全局安装、拷完不自动运行。可选 `--media` 另下约 20 MB 示范 GIF/MP4。

## Recipe / links
- Repo: https://github.com/sloemo01/diorama（710★，MIT）
- npm：https://www.npmjs.com/package/@sloemo/diorama
- Skill：仓库根目录 `SKILL.md`
- 安装（官方推荐，先问路径，默认建议 `~/skills/diorama`）：
  ```bash
  npx @sloemo/diorama ~/skills/diorama
  # 预览：npx @sloemo/diorama --list
  # 也可：npm i @sloemo/diorama && npx diorama
  ```

## Why it made the cut
可加载 `SKILL.md`、安装路径清楚，710★ 说明材料已被反复使用。与本窗收录的 [papercraft](papercraft.md) 都是 Three.js 场景 skill，但 diorama 走像素/卡通模型盒，papercraft 走弹出式剪纸，互不替代。本窗帖子本身几乎无互动，按高星漏收补上。
