# Muse Video Skill（视频创作虚拟剧组）

**Tags:** video, storyboard, preproduction, prompt, skill
**Source:** [@Emad0x1](https://x.com/Emad0x1/status/2122280615613526095) · 2026-11-16
**Engagement:** 发现帖 1 赞 / 36 次展示；仓库 [LuoJiangYong/muse-video-skill](https://github.com/LuoJiangYong/muse-video-skill) 现 94★ / 16 forks，MIT。上游 README 标明「开发中」，最近推送 2026-09-30。

## When to use
有创意但需要专业剧本、分镜、美术方向和可直接给下游视频模型用的提示词时用。它产出开拍前的策划案（Creative Package），不是本地把素材剪成片。已经有分镜、只差 Remotion / FFmpeg 出片，应走 [Remotion Agent Skills](remotion-skills.md) 等成片技能。

## What it does
通用 Agent Skills 格式的「虚拟剧组」：38 个标杆案例技法库 × 导演/编剧/摄影/美术/特效/声音六角色，8+1 阶段管线（含 Director 审核门与 Phase 7.5 模型编译）。导出文学剧本、6/9 宫格分镜、色板与风格参考、图/视频 prompt、字幕与音频 brief，以及面向 Seedance 2.0、ComfyUI、Kling 等的调用指令和成本估算。仓库有完整实测示例（含棚拍广告成片预览）。

## Recipe / links
- Repo: https://github.com/LuoJiangYong/muse-video-skill（MIT，94★）
- 克隆到技能目录，例如 `~/.claude/skills/muse-video/`，或 `hermes skills install muse-video-skill`
- 示例：「帮我策划一个产品广告，风格参考 Apple Don't Blink」
- SKILL.md 在仓库根目录

## Why it made the cut
完整可加载技能：有 SKILL.md、脚本、案例库和可核对的实测成品，使用场景是「策划到模型指令」而不是又一个剪辑工具。社区信号中等（94★），且作者仍标「开发中」、约三个月未推送，当作可用的前期制作配方，而不是已冻结的成品工具。
