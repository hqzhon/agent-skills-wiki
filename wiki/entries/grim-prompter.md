# Grim Prompter（仓库威胁建模）

**Tags:** security, threat-modeling, privacy, appsec, skill
**Source:** [@fngly343149](https://x.com/fngly343149/status/2122994769215496322) · 2026-11-18
**Engagement:** 发现帖约 1 赞 / 1 收藏 / 75 次展示；仓库 [jmanico/grim-prompter](https://github.com/jmanico/grim-prompter) 现 538★，MIT（2026-10-28 建仓）

## When to use
要让编码 agent 对当前仓库做设计级威胁建模：画信任边界、跑 STRIDE / PASTA / LINDDUN 等方法、查隐私与 GDPR/CCPA 覆盖，或评估一次代码改动对已有威胁模型的影响。结论需要能回到代码里核对，而不是一份泛泛的安全建议。

## What it does
只读查看项目，按架构工作流（36 套）和方法/分析提示词（29 个）做结构化审查，把可追溯到证据的 JSON 与 Markdown 报告写到 `threat-model/` 目录。另有独立隐私工作流，专查数据处理和对人的伤害。在 Claude Code 用 `/threat-model`，在 Codex CLI 用 `$threat-model`。

## Recipe / links
- Repo: https://github.com/jmanico/grim-prompter（MIT，538★）
- 安装：先 `git clone https://github.com/jmanico/grim-prompter.git ~/grim-prompter`，再把技能链到 agent 目录（先检查是否已有同名技能，避免重复安装）：
  - Claude Code：`mkdir -p ~/.claude/skills && ln -s ~/grim-prompter/skills/threat-model ~/.claude/skills/threat-model`
  - Codex CLI：`mkdir -p ~/.agents/skills && ln -s ~/grim-prompter/skills/threat-model ~/.agents/skills/threat-model`
- 需保持 clone 位置不变，因为 skill 会引用仓库里的提示词。装完后开新会话。其他宿主可按 README 把项目片段写入 `AGENTS.md`。

## Why it made the cut
安全领域有代表性的作者、完整 SKILL.md 与证据追溯要求，使用场景和安装路径都清楚，不是口号式「让 AI 做安全」。
