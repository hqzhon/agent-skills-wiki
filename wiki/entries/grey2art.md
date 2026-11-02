# Grey2Art（游戏灰盒 → 多风格可玩美术原型）

**Tags:** gamedev, godot, unity, blender, 3d, skill
**Source:** [@yukiben01](https://x.com/yukiben01/status/2117210666381840544) · 2026-11-02
**Engagement:** 仓库 hbzheng0942/grey2art（新开源，星数尚少；README 附多组灰盒 vs 美术版对比视频）

## When to use
已有一个能玩的游戏灰盒（或只有玩法 brief / 参考图），想快速比较几种美术方向、做 vertical slice，或把已有风格延伸到新关卡，同时保证产物仍能在 Godot / Unity 里编辑和运行。

## What it does
Skill `greybox-to-multistyle-art` 让 agent 先做风格探索与场景规划（关键视角、空间布局、资产分工、组装顺序），评审确认成本后再生产：结合 AI 3D 生成（Lux3D / Meshy / Tripo / Rodin / Hi3D 任选）、可复用资产和引擎原生几何组装场景；之后支持局部修改、检查受影响的玩法、断点续做。Blender 负责空间灰盒与几何，Godot/Unity 负责可玩循环与运行时测试。

## Recipe / links
- Repo: https://github.com/hbzheng0942/grey2art · agent 入口：`skills/greybox-to-multistyle-art/SKILL.md`
- 安装：下载 Release 的 skill 包解压后运行 `python3 scripts/install.py --host auto --replace`（支持 Codex、Claude Code、WorkBuddy）
- 依赖：Python 3.11+、Blender、Godot 或 Unity；生成新模型需配置一个 AI 3D 服务（付费生成前会先审成本）
- 示例请求：`Use greybox-to-multistyle-art to turn <project path> into a clay-style playable art prototype.`

## Why it made the cut
有完整 SKILL.md 与安装脚本、场景非常具体（灰盒→多风格可玩原型），README 带可验证的演示视频和流程文档；补足 wiki 里「游戏美术管线」这一类。星数还低，属早期项目，先小项目试用。
