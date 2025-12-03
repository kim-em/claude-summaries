---
source_path: /Users/kim/.claude/skills/merge-conflict-helper
generated: 2025-12-01T21:45:00Z
git_sha: b75fd51d2702e678b15ef7ce28cf6993a31edb62
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# merge-conflict-helper

## Overview

A skill for resolving merge conflicts on GitHub pull requests in Lean/Mathlib projects. Provides a structured workflow for checking out PRs in temp directories, attempting merges with master, analyzing conflicts, auto-resolving obvious cases (import additions, version bumps, sequential additions), and generating detailed resolution logs. Includes heuristics for distinguishing auto-resolvable conflicts from those requiring user review, with emphasis on build verification and documentation.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Complete merge conflict resolution workflow with 9 steps: setup, state verification, merge attempt, conflict analysis, resolution, logging, build verification, user reporting, and push decision |

## Subdirectories

None.

## Search Tags

merge-conflict-resolution github pull-requests lean mathlib git-merge conflict-analysis auto-resolution import-conflicts version-conflicts build-verification resolution-logging workflow lean4 mathlib4 gh-cli lake-build
