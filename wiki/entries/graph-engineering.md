# Graph Engineering

**Tags:** knowledge-graph, task-graph, graphrag, skill, teaching
**Source:** [@Ryrenz](https://x.com/Ryrenz/status/2114705868415467858) · 2026-10-26
**Engagement:** discovery post · repo ~550★ · full SKILL + `/kg-tutor` workflows

## When to use
When prompt-tuning has hit a wall and you need the agent to design **structure**: knowledge graphs (what it remembers) and task graphs (how work fans out, verifies, and stops)—including teaching mode that walks the pipeline on your domain.

## What it does
Claude-compatible skill distilled from SEU’s graduate Knowledge Graph course (npubird/KnowledgeGraphCourse, ~4.4K★): 9-stage KG pipeline (scope → ontology → extract → fuse → GraphRAG) plus task-graph patterns (delete fake edges, diamond workers+verifier, stop rule, human gate). Ships `/kg-tutor` and paste-ready `/kg-*` workflow blocks.

## Recipe / links
- Repo: https://github.com/codejunkie99/graph-engineering (~550★)
- Skill path: `graph-engineering/` (+ `references/`, `WORKFLOWS.md`, `dist/graph-engineering.skill`)
- Install: clone then `cp -r graph-engineering/graph-engineering ~/.claude/skills/`

## Why it made the cut
Full SKILL.md + teaching workflows; clear graph-structure use case; substantial repo grounded in a well-known course (not empty hype).
