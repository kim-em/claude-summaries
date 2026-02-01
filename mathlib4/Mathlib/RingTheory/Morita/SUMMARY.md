---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Morita
generated: 2026-02-01T00:00:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 2
subdirs_count: 0
---

# Morita

## Overview

Formalizes Morita equivalence of rings, a fundamental concept in noncommutative ring theory. Two R-algebras A and B are Morita equivalent if their categories of modules are R-linearly equivalent. The directory establishes that Morita equivalence is an equivalence relation (reflexive, symmetric, transitive), that isomorphic algebras are Morita equivalent, and proves the key theorem that any ring R is Morita equivalent to its matrix ring Mₙ(R).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `MoritaEquivalence R A B` structure and `IsMoritaEquivalent R A B` predicate; proves reflexivity, symmetry, transitivity, and that algebra isomorphisms induce Morita equivalence |
| Matrix.lean | Constructs the categorical equivalence between Mod-R and Mod-Mₙ(R); defines functors `toMatrixModCat` and `toModuleCat`; proves `IsMoritaEquivalent.matrix` showing R ≈ Mₙ(R) |

## Subdirectories

(none)

## Search Tags

Morita-equivalence module-category linear-equivalence matrix-ring noncommutative-ring category-theory R-linear-functor algebra-equivalence Mod-R matrix-module elementary-matrix
