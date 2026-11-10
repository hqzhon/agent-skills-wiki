# image-to-sculpt（按图度量的 3D 雕刻）

**Tags:** 3d, sculpting, blender, image-to-3d, skill
**Source:** [@oaichu95](https://x.com/oaichu95/status/2119626742243504340) · 2026-11-09
**Engagement:** 低互动发现帖 · gokayfem/image-to-sculpt · MIT · 80★

## When to use
当你要让 coding agent **从一张图**（AI 图、渲染、手办/产品照片、线稿，或先 `imagine` 出干净全身图）做出可对着原图核对的 watertight 3D sculpt，并要 Blender 回放/延时摄影证明过程——而不是黑盒 image-to-3D 吐一个无法度量的 mesh。不适合整间房间场景、无图文生 3D、绑骨动画、PBR 贴图或 CAD 精度零件。

## What it does
面向 Claude Code / Codex / Cursor / Copilot / Gemini 的 skill：正面图用 mask、metric depth/焦距、normals 约束；未见侧面先生成再做圆圈配准与筛查；视觉外壳后多轮对 normals / 轮廓 / 深度做 fit；对称、焦点区、缝隙切割与平滑。CLI `scripts/i2s.py` 管脚手架、预算内 fal 调用、配准、雕刻、拟合检查、Blender 回放、转台片与 GLB/OBJ/STL 导出。同作者系列的下一步（在 Video 2 GLSL / Blender Nodes / Physics / CSS 之后）。

## Recipe / links
- Repo: https://github.com/gokayfem/image-to-sculpt （MIT，约 80★）
- Claude Code：`claude plugin marketplace add gokayfem/image-to-sculpt` 后 `claude plugin install image-to-sculpt@image-to-sculpt`；或 `cp -R skills/image-to-sculpt ~/.claude/skills/`
- Skill 路径：`skills/image-to-sculpt/SKILL.md` · CLI：`scripts/i2s.py`

## Why it made the cut
完整 SKILL.md 写清输入路由与边界，配套可验证的测量/回放管线，不是「帮我建个 3D」一句提示；配方具体可复用。
