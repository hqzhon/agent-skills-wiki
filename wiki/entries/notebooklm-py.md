# notebooklm-py（非官方 Gemini Notebook / NotebookLM API 与技能）

**Tags:** unofficial, gemini-notebook, notebooklm, python, cli, research, audio, video, skill
**Source:** [@fngly343149](https://x.com/fngly343149/status/2125170610825527782) · 2026-11-24
**Engagement:** 本窗介绍帖互动很低（1 赞）；仓库 [teng-lin/notebooklm-py](https://github.com/teng-lin/notebooklm-py) 现 20,364★，MIT，有测试 CI，2026-11-24 仍在推送

## When to use
要用编程或编码 agent 操作 **Gemini Notebook**（原 NotebookLM）时用：管理笔记本和资料、做有根据的问答与调研，或生成/下载 Audio Overview、Video Overview 等成品。不要把它当成通用 Gemini API，也不适合无关的内容创作。这是非官方库，走未文档化接口，Google 改接口就可能失效。

## What it does
仓库同时提供 Python 包、\`notebooklm\` CLI 和根目录可加载 [SKILL.md](https://github.com/teng-lin/notebooklm-py/blob/main/SKILL.md)。技能会指导 agent 先安装与鉴权，优先用 CLI 的 \`--json\` 和明确 ID，便于并发下检查每一步；只有在用户要写应用代码、或 CLI 表达不了时，才改用 typed async Python API。README 写明 Google 已于 2026-07 将产品更名为 Gemini Notebook，本包名称仍是 \`notebooklm-py\`，驱动的是同一服务。作者声明部分能力网页 UI 未必暴露。

## Recipe / links
- Repo: https://github.com/teng-lin/notebooklm-py（20,364★，MIT）
- PyPI: https://pypi.org/project/notebooklm-py/
- 安装（Python 3.10+，写入用户现有环境，不要轻易 \`--break-system-packages\`）：
  \`\`\`bash
  pip install "notebooklm-py[browser]"
  npx skills add teng-lin/notebooklm-py
  \`\`\`
  只需 CLI 时也可用 \`uv tool install "notebooklm-py[browser]"\` 或 pipx。可选 \`notebooklm-py[cookies]\` 做浏览器 cookie 提取。
- Skill: 仓库根目录 \`SKILL.md\`（name: \`notebooklm\`）
- 注意：非官方、未文档化 API，鉴权通常依赖浏览器登录或 cookie，请先读 README 的风险说明和技能里的凭据处理规则。

## Why it made the cut
高星漏收：可加载 \`SKILL.md\`、明确使用边界、CLI/API 双路径和测试 CI 都齐，场景清楚（把 Gemini Notebook 交给 agent 跑，而不是再买一个聊天包装）。本窗互动很低，按仓库信号补上。必须标明非官方和接口可能变动，不能写成 Google 官方技能。
