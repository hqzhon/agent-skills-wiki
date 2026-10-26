# Chaperone（Baker lab / RosettaCommons）

**Tags:** science, protein-design, skill-pack, hpc, slurm
**Source:** [@toolomeai](https://x.com/toolomeai/status/2114556640892461119) · 2026-10-26
**Engagement:** directory mention; repo ~135★

## When to use
When the user is running **protein design / folding / analysis campaigns** with coding agents and needs reproducible SLURM pipelines plus on-demand agent skills (setup, design, blocks, visualize, etc.).

## What it does
Unified structural-biology harness (RFD3, BindCraft, AF3, ProteinMPNN, …) with `AGENTS.md` routing and a pack under `.agents/skills/` (`setup`, `design`, `build-block`, `auto-research`, `slurm-*`, `visualize`, …). Root `SKILL.md` tells the agent to read AGENTS.md then load only task-relevant skills.

## Recipe / links
- Repo: https://github.com/RosettaCommons/chaperone (~135★, MIT)
- Toolome card: https://toolome.bio/tools/chaperone/
- Preprint: https://doi.org/10.64898/2026.10.19.759896

## Why it made the cut
Ships many real SKILL.md files plus AGENTS.md routing for a clear scientific workflow—not “AI for biology” vapor.
