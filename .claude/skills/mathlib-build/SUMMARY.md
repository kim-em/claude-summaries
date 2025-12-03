---
source_path: /Users/kim/.claude/skills/mathlib-build
generated: 2025-12-01T13:15:00Z
git_sha: b75fd51d2702e678b15ef7ce28cf6993a31edb62
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# mathlib-build

## Overview

A Claude Code skill that provides best practices for building Mathlib and large Lean projects with reduced output verbosity. The skill instructs Claude to use `lake build -q --log-level=info` to suppress per-file build progress messages while preserving diagnostic output (errors, warnings, and info messages). This is critical for Mathlib builds which touch thousands of files and would otherwise consume excessive tokens and obscure actual build issues.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill definition with frontmatter and detailed flag explanations, output behavior table, and usage examples |

## Subdirectories

None.

## Search Tags

mathlib lake build quiet verbosity logging lean4 build-flags diagnostics errors warnings info-messages token-optimization build-output
