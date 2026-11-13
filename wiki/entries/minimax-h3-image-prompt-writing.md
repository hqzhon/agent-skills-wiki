# h3-image-prompt-writing（MiniMax 官方，H3-Image 提示词技能）

**Tags:** image-generation, prompt-writing, minimax, official, design
**Source:** [@Lonely__MH](https://x.com/Lonely__MH/status/2120869218602402209) · 2026-11-12
**Engagement:** 38 赞 / 63 收藏 / ~4k 曝光；随 MiniMax-AI/MiniMax-H3-Image 开源仓库（~300★，2026-11-09 建仓）发布

## When to use
用 MiniMax-H3-Image 出图或改图（海报、信息图、图表、产品图、UI、角色、分镜等），只想说一句想法，让 Claude Code / Codex 自动写成符合模型偏好的完整英文长提示词，并可直接调用 API 出图。

## What it does
- 按「任务 → 版式 → 画幅 → 主体 → 风格 → 文字」的顺序把短需求扩写成完整画面描述
- 规则：先写任务再写风格、先布局后细节、用可见细节（光、材质、颜色）代替「高级感」之类的空词；图中出现的文字原样加引号并写明位置与层级；无字时明确声明
- 支持编辑模式：最多 16 张参考图，按 `<Picture 1>`、`<Picture 2>` … 顺序引用
- 附 `references/t2i-en.txt`、`references/edit-en.txt` 示例指南；`scripts/generate.py` 读取 `MINIMAX_API_KEY` 直接渲染（国内平台 key 需设 `MINIMAX_API_BASE=https://api.minimax.cn`）；没有 key 时只交付提示词

## Recipe / links
- 技能目录：https://github.com/MiniMax-AI/MiniMax-H3-Image/tree/main/skills/h3-image-prompt-writing
- 安装：
  ```bash
  npx skills add https://github.com/MiniMax-AI/MiniMax-H3-Image --skill h3-image-prompt-writing
  ```

## Why it made the cut
模型厂商官方随模型发布的提示词技能，SKILL.md、参考示例和渲染脚本都在仓库里可核；场景明确，也是「把官方 Prompting Tips 固化成技能」的好范本。注意仓库许可证在 GitHub 上显示为 NOASSERTION，商用前请看仓库 LICENSE。
