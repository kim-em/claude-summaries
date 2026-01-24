---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean/Elab/Tactic
generated: 2026-01-24T23:47:30Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Tactic

## Overview

The `Mathlib/Lean/Elab/Tactic/` directory provides utilities that extend Lean 4's tactic elaboration infrastructure. It contains helper functions for working with tactic goals and running tactics in MetaM contexts, supporting Mathlib's metaprogramming needs during tactic elaboration.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Extends `Lean.Elab.Tactic.Basic` with `getMainTarget''` - returns the expected type for the main goal after cleaning up annotations using `MVarId.getType''` (similar to `getType'` but uses `cleanupAnnotations` instead of `whnf`) |
| Meta.lean | Extends `Lean.Elab.Tactic.Meta` with `runTactic'` - applies tactic code to an mvar in MetaM, a variant of `Lean.Elab.runTactic` that forgets the final `Term.State` |

## Subdirectories

None

## Search Tags

lean4 tactic elaboration metam goal-management tactic-execution mvar annotations type-inference mathlib-infrastructure metaprogramming
