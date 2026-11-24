# OmniCAD Skill（有证据的二维 CAD 出图与校对）

**Tags:** cad, autocad, dxf, dwg, engineering, python, skill
**Source:** [@CommunismHaruh1](https://x.com/CommunismHaruh1/status/2125106497118228685) · 2026-11-24
**Engagement:** 本窗为安装说明帖（9 赞 / 3 转发）；仓库 [Haruhi764/OmniCAD-Skill](https://github.com/Haruhi764/OmniCAD-Skill) 现 24★，MIT，含单元测试与验收记录

## When to use
要把已经核对过的尺寸和修改范围，做成可编辑的 2D CAD（DXF，或在 Windows 授权 AutoCAD 里做原生 DWG/PDF），并且需要留下来源和验收依据时用。它不负责从照片 OCR 矢量化，也不做 BIM、3D 或其他 CAD 厂商适配；不会仅凭专业领域名称去补缺失尺寸或给出合规结论。

## What it does
根目录 [SKILL.md](https://github.com/Haruhi764/OmniCAD-Skill/blob/main/SKILL.md) 加上 \`omnicad\` CLI。流程包括：把用户请求与参考资料里的指令分开（\`omnicad intent\`）、清点输入（\`intake\`）、用清单或轴/法兰配方编译作业、\`build\` 出 DXF、按 \`light\` / \`standard\` / \`full\` 做结构与证据验收（\`oqa\`）、再 \`publish\`。机械向示例可生成阶梯轴、带凸台法兰等，并附 AutoCAD 2023 实测预览。原生 DWG/PDF 依赖 Windows、已授权 AutoCAD、字体和出图设置。

## Recipe / links
- Repo: https://github.com/Haruhi764/OmniCAD-Skill（24★，MIT）
- 需要 Python 3.10+。在仓库里：
  \`\`\`bash
  python -m pip install ".[intake,autocad]"
  npx skills add Haruhi764/OmniCAD-Skill
  \`\`\`
  纯 DXF 用基础包即可；PDF/图片预检要 \`intake\` 附加依赖。Skill 与 CLI 可分开用。
- 中英 README、\`references/validation.md\` 与 \`examples/\` 可对照。

## Why it made the cut
不是「让模型直接画一张图」，而是把已复核尺寸、修改范围和验收证据写成可加载配方，有 CLI、测试和实测出图样例。24★ 不算高，但场景、步骤和边界都写清楚了，本窗也有可核对的安装说明。原生 AutoCAD 路径的平台限制要在条目里标明。
