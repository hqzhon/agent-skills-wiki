# Open Code Review（阿里官方：确定性规则 + LLM 代码审查）

**Tags:** official, alibaba, code-review, cli, skill-pack
**Source:** [@sodnaso](https://x.com/sodnaso/status/2125802867730878824) · 2026-11-26；同窗亦见于周榜盘点 [@edinsoncode](https://x.com/edinsoncode/status/2125779136727663072)
**Engagement:** 介绍帖互动低；周榜帖 3 赞 / 3 收藏。仓库 [alibaba/open-code-review](https://github.com/alibaba/open-code-review) 现 56,426★ / 4,665 forks，Apache-2.0，2026-11-26 仍有推送。

## When to use
要给工作区改动、PR、commit 或分支对比做**行级**代码审查，并且希望规则检查（空指针、线程安全、XSS、SQL 注入等）和 LLM 判断分开配置时用。不要用它代替合并决定，也默认不要让它直接改代码（技能写明：只在你明确要求时才修）。和已收录的 [reviewing-pr-decisions](reviewing-pr-decisions.md)（关注判断点而不是逐行评论）互补。

## What it does
阿里巴巴内部 AI 代码审查助手的开源版（README：两年服务数万开发者）。核心是 `ocr` CLI：读 Git diff，按流水线 + 可配置模型（Anthropic / OpenAI / Bedrock 等）给出带行号的意见，也可 `ocr scan` 审整文件。Agent Skills 有两种模式：

- `open-code-review`：走 OCR 自带审查流水线和独立配置的模型；
- `open-code-review-delegate`：仍用 OCR 的流程和护栏，但模型用当前编码 agent 已有的凭证。

两种模式都需要 Git >= 2.41 和 `ocr` CLI；原生模式还要单独配 OCR 的模型端点。审查 GitHub PR 时需要 Python 3 和已登录的 `gh`。

## Recipe / links
- Repo: https://github.com/alibaba/open-code-review（56,426★，Apache-2.0）
- 站点：https://open-codereview.ai
- 安装技能：`npx skills add alibaba/open-code-review`
- 预装 CLI：`npm install -g @alibaba-group/open-code-review`
- 技能：[skills/open-code-review/SKILL.md](https://github.com/alibaba/open-code-review/blob/main/skills/open-code-review/SKILL.md)、[skills/open-code-review-delegate/SKILL.md](https://github.com/alibaba/open-code-review/blob/main/skills/open-code-review-delegate/SKILL.md)

## Why it made the cut
可加载官方技能 + 可验证的大规模审查工具，56k★、Apache-2.0，使用场景和安装路径清楚。本窗为高星漏收。需自备模型端点（或改用 delegate 模式走宿主 agent）。
