---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Logic/Equiv/Fin
generated: 2026-01-25T23:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Fin

## Overview

The `Fin/` subdirectory provides specialized equivalences involving `Fin n` (finite types with `n` elements). It contains fundamental constructions for converting between `Fin n` and related types (like `Option (Fin (n-1))` or sum types), product/sum decomposition equivalences, and cyclic permutation operations on finite types. These equivalences are building blocks for working with finite sets, permutations, and indexed families in Lean/mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `Fin n` equivalences: `finSuccEquiv` (`Fin (n+1) ≃ Option (Fin n)`), `finSuccEquiv'` (generalized removal of arbitrary element), `finSuccAboveEquiv` (order isomorphism via `succAbove`), `finSumFinEquiv` (`Fin m ⊕ Fin n ≃ Fin (m+n)`), `finSumNatEquiv` (`Fin n ⊕ ℕ ≃ ℕ`), `finAddFlip` (rotation equivalence `Fin (m+n) ≃ Fin (n+m)`), `finProdFinEquiv` (`Fin m × Fin n ≃ Fin (m*n)`), division/modulo equivalences for ℕ and ℤ, `Fin.castLEquiv` (subtype embedding), `Fin.appendEquiv` (function concatenation), and `embeddingFinSucc` (decomposition of embeddings from `Fin (n+1)`); 411 lines |
| Rotate.lean | Cyclic permutations on `Fin n`: `finRotate` (one-step right rotation, the cycle `(0, 1, ..., n-1)`), `finCycle k` (rotation by `k` steps, equivalent to iterating `finRotate`), lemmas about rotation behavior at boundaries (last element maps to 0), connections between `Fin.snoc` and `Fin.cons` via rotation, and inequalities characterizing rotation effects; authored by Paul Lezeau, Lawrence Wu, Jeremy Tan; 133 lines |

## Subdirectories

None

## Search Tags

fin finite-types equivalence option-fin sum-fin product-fin rotation cyclic-permutation fintype fin-equiv casting embedding division-modulo lean4 mathlib
