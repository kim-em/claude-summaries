---
source_path: /Users/kim/.claude/skills/lean-mwe
generated: 2026-01-24T21:00:00Z
git_sha: a7f9d0e5692aa0d2ec137abd8f2601dccd0a21ec
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# lean-mwe

## Overview

A Claude Code skill that provides systematic methodology for minimizing Lean errors into minimal working examples (MWEs) suitable for bug reports. The skill emphasizes a disciplined, guard-first approach: setting up `#guard_msgs` or `fail_if_success` BEFORE any minimization begins, then iteratively removing code while verifying the guard still passes. Core principles include minimizing in place (not creating separate MWE files), never changing the toolchain, making one change at a time, and using mechanical inlining to eliminate ALL imports—reaching pure Lean 4 proves bugs belong in the lean4 repository. Includes comprehensive testing scenarios and validated examples.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Comprehensive 500-line minimization methodology: critical guard-first discipline, checking current directory before cloning, never changing toolchain, minimize in place not in separate files, systematic reduction strategies with expanded guidance—repeatedly inspect goal states with `done` after every change before the error, leverage proof irrelevance to always replace proofs with `sorry` (never refactor), progressively sorry-ify proofs from leaf cases inward, sorry dependent proofs before removing attributes, simplify structures by removing fields and default values, replace universe-polymorphic types (Sort u/Type u) with concrete Type, mechanical inlining proving "inlining always works", one-change-at-a-time discipline, and backtracking with git commits |
| TESTING.md | Four concrete test examples for validating the skill: diseq_cancel_var kernel error in nightly-testing-2025-11-27, grind metadata cleanup issue after double norm_cast at v4.26.0-rc1, grind +revert requirement for descFactorial in nightly-testing-2025-11-21, and compiler panic in UnreachableBranches at specific commit |
| VALIDATION.md | Reference solutions for all four test cases, showing the final minimized code that reproduces each error with minimal dependencies |

## Subdirectories

None

## Search Tags

lean4 mwe minimal-working-example bug-reports error-minimization guard_msgs tactic-failures kernel-errors grind compiler-panics mathlib testing reduction backtracking systematic-debugging reproducible-examples
