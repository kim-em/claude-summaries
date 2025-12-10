---
source_path: /Users/kim/.claude/skills/merge-conflict-helper
generated: 2025-12-11T12:00:00Z
git_sha: 5a5c7bc8574841a2870eff76b15c9a7bf9b3c3fa
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# merge-conflict-helper

## Overview

A skill for resolving merge conflicts on GitHub pull requests in Lean/Mathlib projects. Provides a structured 10-step workflow: setup (temp directory, gh pr checkout), state verification (lake exe cache get, build), merge attempt, conflict analysis, resolution, resolution log creation, build verification with iterative fixes, user report generation, push target determination (handling fork-based vs same-repo PRs), and push confirmation. Includes detailed heuristics for auto-resolvable conflicts (import additions, version bumps, sequential lemma additions, whitespace, Mathlib.lean) versus those requiring user review (same theorem modified both sides, API changes affecting PR logic, complex proofs). Provides example output templates for both successful and uncertain resolutions.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Complete merge conflict resolution workflow with 10 steps covering checkout, verification, merge, analysis, resolution, logging, build verification, reporting, push target determination, and push confirmation. Includes auto-resolve vs manual-review heuristics, common Mathlib patterns, when-to-stop criteria, and resolution log template |

## Subdirectories

None.

## Search Tags

merge-conflict-resolution github pull-requests lean mathlib git-merge conflict-analysis auto-resolution import-conflicts version-conflicts build-verification resolution-logging workflow lean4 mathlib4 gh-cli lake-build fork-handling push-target
