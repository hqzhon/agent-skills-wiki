# repo-vet（安装前只读审查仓库与软件包）

**Tags:** security, supply-chain, audit, skill
**Source:** [@usuallyazu](https://x.com/usuallyazu/status/2123218900838146521) · 2026-11-19
**Engagement:** 作者自荐帖（0 赞）；仓库 [azudev4/repo-vet](https://github.com/azudev4/repo-vet) 0★，MIT。早期条目。

## When to use
安装某个 GitHub/GitLab 仓库、npm/PyPI/crates.io 包、VS Code 扩展或发行版安装包**之前**，想先搞清它能对你的机器做什么、源码和真实二进制是否一致时使用。也适用于「这个 Discord 模组/客户端安全吗」这类问题。

## What it does
Claude Code 技能：先跑确定性扫描，再按档位拉起并行「镜头」agent（low 约 3–6，medium 默认 10–16，high 20–40），默认怀疑、要证据。覆盖安装期自执行（postinstall、hooks、devcontainer 等）、隐藏/不可见代码、窃密与回连、持久化，以及「源码开源但 .exe 不一样」的发行包对照。硬规则是**永不执行、构建或安装目标**；克隆落在 `~/.repo-vet/targets/`，避免当前会话自动加载目标的 `CLAUDE.md` / hooks / MCP。

## Recipe / links
- Repo: https://github.com/azudev4/repo-vet（MIT，0★）
- 安装（Claude Code 插件，推荐）：
  ```
  /plugin marketplace add azudev4/repo-vet
  /plugin install repo-vet@repo-vet
  ```
  然后 `/repo-vet:repo-vet <target> [low|medium|high]`，或直接问「这个仓库安装前安全吗？」。也可把 `skills/repo-vet` 拷到 `~/.claude/skills/repo-vet`。
- 依赖：Node 18+、git。可选 7-Zip、已登录的 `gh`、`VT_API_KEY`（只做哈希查询、不上传文件）；若本机已有 osv-scanner、gitleaks 等会顺便用，技能本身不会代装。
- 示例：`/repo-vet https://github.com/someone/cool-discord-mod high` 或 `/repo-vet npm:some-package@1.2.3`

## Why it made the cut
和已有的 SkillSpector / aig-skill-scan 不同：对象不限于 skill 包，而是安装前的仓库与软件包供应链，并且把「只读、不执行、隔离克隆」写进流程。仓为 0★，属早期收录，装前仍建议先读脚本。
