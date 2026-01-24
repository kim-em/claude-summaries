---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Coxeter
generated: 2026-01-24T23:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 4
subdirs_count: 0
---

# Coxeter

## Overview

The `Coxeter/` directory provides a comprehensive formalization of Coxeter groups and Coxeter systems. Coxeter groups are defined via presentations with generators (simple reflections) and relations determined by a Coxeter matrix. The formalization includes the fundamental theory of length functions, reduced words, descents, reflections, and inversions. Coxeter matrices (symmetric matrices with diagonal entries 1 and off-diagonal entries ≠ 1) are defined along with standard examples from Lie theory (types A, B, D, E, F, G, H, I).

## Key Files

| File | Purpose |
|------|---------|
| Matrix.lean | Coxeter matrices: symmetric matrices with diagonal 1 and off-diagonal ≠ 1; standard types (Aₙ, Bₙ, Dₙ, E₆, E₇, E₈, F₄, G₂, H₃, H₄, I₂ₘ) |
| Basic.lean | Core definitions: CoxeterMatrix.Group, CoxeterSystem, IsCoxeterGroup, simple reflections, universal property (lift), words, wordProd, alternatingWord, braid relations |
| Length.lean | Length function on Coxeter groups: reduced words, length parity, descents (left/right), triangle inequality for length, length-one characterization |
| Inversion.lean | Reflections, left/right inversions, inversion sequences: IsReflection, IsLeftInversion, IsRightInversion, leftInvSeq, rightInvSeq, nodup property for reduced words |

## Subdirectories

(No subdirectories)

## Search Tags

coxeter-group coxeter-system coxeter-matrix simple-reflection length-function reduced-word descent inversion reflection alternating-word braid-relation presentation matrix-type lie-theory weyl-group artin-tits
