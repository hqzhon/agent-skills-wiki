# fab-asset-prep（把 AI 三维模型整理成 Fab 上架包）

**Tags:** 3d, blender, fab, gamedev, marketplace, skill
**Source:** [@LamineBelhadj4](https://x.com/LamineBelhadj4/status/2126456247821926410) · 2026-11-28
**Engagement:** 作者第一方介绍帖 1 赞；仓库 [LamineBelhadj/fab-asset-prep](https://github.com/LamineBelhadj/fab-asset-prep) 当天新建，现 0★，MIT。

## When to use
已经有了 AI 生成的三维模型，要在 Blender 里修到能上 Fab（或同类资产商店）时用：真实世界尺度、干净的 FBX/GLB/Blender 压缩包、校验，以及诚实的上架文案和渲染图。它不负责从零生成模型，也不保证商店审核一定通过。

## What it does
技能目录 [fab-asset-prep/SKILL.md](https://github.com/LamineBelhadj/fab-asset-prep/blob/main/fab-asset-prep/SKILL.md) 加上脚本，大致流程是：修复网格与变换、统一真实尺度、导出并打包（每个格式一个根目录 zip）、在干净场景里重新导入做校验（网格数量、尺寸、贴图、UV，并扫描残留的用户名/OneDrive/UUID 等痕迹）、渲染前后对比和上架图，再按 `references/listing.md` 写标题、描述、标签和定价提示。校验失败要如实报告，看起来更差的修复要回退。

## Recipe / links
- Repo: https://github.com/LamineBelhadj/fab-asset-prep（0★，MIT）
- 技能路径：`fab-asset-prep/SKILL.md`
- 安装：
  ```bash
  npx skills add LamineBelhadj/fab-asset-prep
  ```
- 需要本机 Blender；仓库还带 `scripts/` 与 `references/`。

## Why it made the cut
第一方发布，上架前的修复、打包、校验和文案步骤都很具体，有 SKILL.md 和 MIT 许可。星标和互动都还是零，但对「AI 模型怎么送到资产商店」这条场景来说，配方已经可执行，故收录并标明信号仍弱。
