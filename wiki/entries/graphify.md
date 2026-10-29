# Graphify（/graphify 知识图谱 Skill）

**Tags:** knowledge-graph, codebase, cli, skill, local-first
**Source:** [@KeyoAPI](https://x.com/KeyoAPI/status/2115679485488148832) · 2026-10-29
**Engagement:** ~138k★ · Apache-2.0 · AST graph, not a vector store

## When to use
When agents **re-grep the whole repo every session** and you want a local, queryable knowledge graph of code (+ optional docs/PDF/media) so the assistant can `query` / `path` / `explain` instead of blind search.

## What it does
CLI `graphify` + assistant skill: tree-sitter AST maps ~40 languages locally (no LLM for code), writes `graph.html` / `GRAPH_REPORT.md` / `graph.json`, then supports path/explain/query. `graphify install` registers the skill for Claude Code, Cursor, Codex, Gemini CLI, Copilot, and many more. Optional semantic pass for docs/media; Cloud product is separate.

## Recipe / links
- Repo: https://github.com/Graphify-Labs/graphify (~138k★, Apache-2.0)
- Install CLI: `uv tool install graphifyy` then `graphify install` (or `--project`)
- In-assistant: `/graphify .` (Codex: `$graphify`)
- Docs: https://docs.graphify.com · PyPI package name is `graphifyy`

## Why it made the cut
Installable skill + CLI with clear when-to-use, local-first recipe, and a large verifiable open-source codebase.
