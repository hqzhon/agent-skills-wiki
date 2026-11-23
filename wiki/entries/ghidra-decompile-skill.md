# ghidra-decompile-skill（按地址做 Ghidra 定向反编译）

**Tags:** security, reverse-engineering, ghidra, decompiler, skill
**Source:** [@lcheylus](https://x.com/lcheylus/status/2124776238636003682) · 2026-11-23
**Engagement:** 发现帖 1 赞 / 1 转发 / 2 收藏；仓库 [ioma8/ghidra-decompile-skill](https://github.com/ioma8/ghidra-decompile-skill) 44★ / 4 forks，MIT

## When to use
要用 Ghidra 对已知地址做定向反编译、交叉引用或 vtable/RTTI 转储，并且想避开整包自动分析的长时间开销；或 GhidraMCP 扩展与 Ghidra 版本不匹配、反编译全部失败时需要修复步骤。已有常驻 RPC 守护进程方案时，见 [ghidra-rpc](ghidra-rpc.md)。

## What it does
核心观点是「成本在分析，不在反编译」：对一份 114 MB 的去符号 AArch64 镜像，`-noanalysis` 导入一次后，定向反编译一个函数约 3.3 秒，全量自动分析则可能数小时。SKILL.md 给出选路（无项目的一两次查询 / 保留工程反复问 / 打开 GUI + MCP / 整包伪代码扫描）、把文件偏移钉到镜像基址、无头按地址反编译，以及 22 个配套脚本（按地址反编译、vtable/RTTI、xrefs、AArch64 `PACIASP` 入口扫描等）。另外记录了 GhidraMCP 7.0.0 针对 12.1.4、在 12.2 上会因 `SleighLanguageDescription` 失败，需改用 `chore/ghidra-12.2` 分支并确认 `extension.properties` 的版本号。

## Recipe / links
- Repo: https://github.com/ioma8/ghidra-decompile-skill（44★，MIT）
- 安装：`npx skills add ioma8/ghidra-decompile-skill`（可选 `-g`）；再把 `tools/*.java` 拷到 `~/ghidra_scripts`，或在无头运行时用 `-scriptPath`
- 前置：Ghidra（作者在 12.2 上验证）。无头路径不需要 MCP；桥接路径需要 [bethington/ghidra-mcp](https://github.com/bethington/ghidra-mcp) 和 `uv`

## Why it made the cut
和已收录的 [ghidra-rpc](ghidra-rpc.md)（Cellebrite Labs，常驻守护进程 + CLI）不是同一套工具：这边强调「导入一次、按地址反编译」和 MCP 版本错配修复，脚本与计时可核对。只用于分析自己有权处理的二进制。
