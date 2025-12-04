---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Pointwise
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Pointwise

## Overview

The `Pointwise/` directory contains theory for stabilizers of sets under pointwise group actions. The single file characterizes when group elements fix a set under the natural action, providing fundamental results about set stabilizers, subgroup stabilizers, and finset stabilizers with applications to quotient groups.

## Key Files

| File | Purpose |
|------|---------|
| Stabilizer.lean | Characterizes stabilizer subgroups for sets/finsets under group actions: `stabilizer G s` consists of elements preserving membership (`a • b ∈ s ↔ b ∈ s`), proves `stabilizer G (s : Subgroup) = s`, shows stabilizers of finite nonempty sets are finite, establishes `s * stabilizer G s = s` for commutative groups, and proves quotient stabilizer triviality `stabilizer (G ⧸ stabilizer G s) (q '' s) = ⊥` |

## Subdirectories

*(none)*

## Search Tags

pointwise algebra group-action stabilizer subgroup finset quotient-group set-theory mulaction
