# Autoresearch（Claude Autoresearch）

**Tags:** iteration-loop, verification, claude-code, opencode, codex, skill-pack
**Source:** [@bkdgiffug](https://x.com/bkdgiffug/status/2114698055631163634) · 2026-10-26
**Engagement:** ZH explainer · repo ~6.7K★ · multi-agent install

## When to use
When a coding agent should **iterate overnight on a measurable goal** (coverage, bundle size, failing tests)—set goal/scope/metric/verify, then modify → verify → keep/revert—without babysitting every round. Skip if the metric is gameable or flaky.

## What it does
Agent skill inspired by Karpathy’s autoresearch (not the training script): bounded loops with mechanical verification and auto-rollback; orchestrator mode for plain-language goals; subcommands for plan/debug/fix/security/ship/scenario/predict/learn/reason/probe/improve/evals/regression. Claude Code hooks for guardrails; also OpenCode and Codex ports.

## Recipe / links
- Repo: https://github.com/uditgoenka/autoresearch (~6758★)
- Install: `npx skills add uditgoenka/autoresearch` or `/plugin marketplace add uditgoenka/autoresearch`
- Also: `./scripts/install.sh --claude|--opencode|--codex`

## Why it made the cut
Explicit SKILL + commands; clear quantified-iteration use case; large verified multi-harness repo with safety defaults.
