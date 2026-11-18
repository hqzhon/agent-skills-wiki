# 3dviz-pro-max（一句话做可逛 3D 场景）

**Tags:** 3d, threejs, blender, visualization, skill
**Source:** [@aigljrzj](https://x.com/aigljrzj/status/2122947080247476665) · 2026-11-18
**Engagement:** 发现帖互动很低（2 赞 / 58 次展示）；仓库 [viettranx/3dviz-pro-max](https://github.com/viettranx/3dviz-pro-max) 现 1,410★，MIT（2026-09-10 建仓；最近推送停在 2026-09-11）

## When to use
想从一句话做出一个能逛、能看的 Three.js / Blender 3D 场景（小村庄、解剖、光影练习等），但不想自己先选定渲染器、规格和验收方式。

## What it does
十步工作流：选美术方向、定规则、加会动的生物、渲染后再逐帧验收。仓库带配方目录、可运行的 Three.js 模板、37 个英语案例研究，以及展示页 [3dviz.dev](https://3dviz.dev)。必须拷贝整个 `skills/3dviz-pro-max/` 文件夹，不要只拷 `SKILL.md`。作者写明：插件市场安装路径尚未充分测试，首页村子动图是旧素材，不是本技能的实测输出。

## Recipe / links
- Repo: https://github.com/viettranx/3dviz-pro-max（MIT，1,410★）
- 站点: https://3dviz.dev
- 推荐：`git clone` 后把整个 `skills/3dviz-pro-max` 拷到 agent 的 skills 目录（Claude Code 可用 `ln -s "$(pwd)/skills/3dviz-pro-max" ~/.claude/skills/3dviz-pro-max`）
- 插件市场（README 称仓库需先发布且未经充分测试）：`/plugin marketplace add viettranx/3dviz-pro-max` → `/plugin install 3dviz-pro-max@3dviz-pro-max`
- 案例：克隆后 `cd examples && pnpm install && pnpm dev`

## Why it made the cut
有完整 SKILL.md、可跑案例和诚实的兼容性说明，使用场景清楚。仓已两月未推送，安装前先核对 README 里的限制。
