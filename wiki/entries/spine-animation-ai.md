# Spine Animation AI（从素材绑定并生成 Spine 2D 动画）

**Tags:** animation, spine, gamedev, rigging, claude, skill
**Source:** [@dextune](https://x.com/dextune/status/2125567678152872165) · 2026-11-25
**Engagement:** 本窗 477 赞 / 63 转发 / 667 收藏；仓库 [GenielabsOpenSource/spine-animation-ai](https://github.com/GenielabsOpenSource/spine-animation-ai) 现 786★ / 114 forks，[PolyForm Noncommercial 1.0.0](https://github.com/GenielabsOpenSource/spine-animation-ai/blob/main/LICENSE)

## When to use
已有 2D 角色素材（分件 PNG、图集，或一张完整立绘），要让 agent 帮你做 Spine 4.2 骨骼绑定，并生成 idle / walk / run / attack / wave / jump 等动画和可在浏览器打开的预览时用。它处理定位、骨骼层级、绘制顺序和关键帧，不是通用生成式视频，也不替代 Esoteric 的 Spine 编辑器做精细调优。商用前先看许可：非商业用途免费，商业使用需另向 [Genielabs](https://genielabs.tech) 授权。

## What it does
根目录 `SKILL.md`（由模板注入 4 个 Python 脚本）指导 Claude：用 SIFT + RANSAC（失败则模板匹配）对照参考图摆放部件，分析遮挡以确定 Z 序，按动画 12 原则写关键帧，导出 Spine 兼容的 `.json` + `.atlas` + `.png`，并用官方 Spine Web Player 生成无需服务器的 `preview.html`。只有一张完整立绘时，`split_character.py` 可走 Gemini 拆成透明分件（需 `GEMINI_API_KEY`）。仓库还带 Reskin Studio：用一句话重绘已绑定角色的贴图并切回各槽位。示例角色 Sombrero 有[在线预览](https://GenielabsOpenSource.github.io/spine-animation-ai/demo/sombrero_idle.html)和部件编辑器。

## Recipe / links
- Repo: https://github.com/GenielabsOpenSource/spine-animation-ai（786★，PolyForm Noncommercial 1.0.0）
- SKILL.md：https://github.com/GenielabsOpenSource/spine-animation-ai/blob/main/SKILL.md
- 推荐（任意 Claude 账号）：把 `SKILL.md` 全文粘进 claude.ai 的 Project Knowledge，上传素材后描述要的动画
- 支持挂载技能目录的环境：
  ```bash
  git clone https://github.com/GenielabsOpenSource/spine-animation-ai.git /mnt/skills/user/spine-animation
  ```
- 也可不经 Claude，按 README 的 Option C 直接跑 `scripts/`（定位 / 建 JSON / 打包图集）
- 依赖：`opencv-python`、`Pillow`、`numpy`；拆分完整立绘时还要 `google-generativeai` 和 Gemini API key

## Why it made the cut
场景清楚（2D 游戏角色绑定与循环动画），有可加载 SKILL.md、脚本、演示成片和在线预览，786★ 且本窗互动很高。许可不是 MIT：条目按非商业配方收录，商用需另授权，拆分立绘还会调用 Gemini。
