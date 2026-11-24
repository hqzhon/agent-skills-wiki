# fast-anything（只把最慢的那 5% 迁到 Rust 并对照验证）

**Tags:** rust, performance, profiling, migration, cli, mcp, skill
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2125190362742374569) · 2026-11-24
**Engagement:** 本窗为技能圈盘点帖（1 赞）；仓库 [EL4CTEO/fast-anything](https://github.com/EL4CTEO/fast-anything) 现 3,425★，MIT，有 CI，npm / crates.io 同步发布

## When to use
Python / Node / TypeScript / Ruby / Java / Go / PHP / C / C++ / C# 等程序变慢，想加速又不必整仓重写成 Rust 时用。它只处理 profiling 里真正热的纯函数（技能建议跳过占比不足约 2% 的部分）。

## What it does
可加载技能 \`skills/fast-anything/SKILL.md\`，并配 CLI 与同名 MCP 工具。循环是：\`scan\` 在用户真实工作负载下找出热点 → \`port\` 录制最多约 500 次真实调用并生成 Rust 桩和 \`TASK.md\` → 由 agent 编写 Rust → \`verify\` / \`enable\` / \`bench\` 证明端口与原函数结果一致后再切换。目标是「只改最慢的 5%」，而不是把整套业务逻辑搬到 Rust。

## Recipe / links
- Repo: https://github.com/EL4CTEO/fast-anything（3,425★，MIT）
- 安装技能：\`npx skills add EL4CTEO/fast-anything\`
- CLI：\`npx @el4cteo/fast-anything\` 或 \`cargo install fast-anything\`（也有 Claude Code 插件）
- Skill: [skills/fast-anything/SKILL.md](https://github.com/EL4CTEO/fast-anything/blob/main/skills/fast-anything/SKILL.md)

## Why it made the cut
高星漏收：配方完整（测量 → 录制 → 改写 → 对照 → 启用），有 CLI/MCP/CI，使用场景清楚。和已收录的 [rust-anything](rust-anything.md)（一块块迁到 Rust、先录像再对照）同类但更窄：这边强调只移植热点纯函数，并明确跳过占比过低的路径。本窗只是盘点提到，按仓库信号补上。
