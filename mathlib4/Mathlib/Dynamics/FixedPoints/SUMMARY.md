---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics/FixedPoints
generated: 2025-01-24T20:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# FixedPoints

## Overview

The `FixedPoints/` directory provides foundational definitions and theorems for fixed points of self-maps. It defines the predicate `IsFixedPt f x` (meaning `f x = x`) and the set `fixedPoints f` of all fixed points. The directory includes algebraic properties (interaction with composition, iteration, semiconjugacy, permutations), topological properties (closedness, convergence of iterates), and a specialized result about Prufer subgroup invariance used in circle dynamics.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `IsFixedPt f x := f x = x` and `fixedPoints f`; lemmas for composition, iteration, semiconjugacy, permutation powers; bijection between fixed points of `f . g` and `g . f` |
| Prufer.lean | Proves that sets invariant under `x -> x^n` preimage are also invariant under pointwise action of the Prufer subgroup (elements with `g^(n^j) = 1`); used in circle rotation dynamics |
| Topology.lean | Topological results: `isFixedPt_of_tendsto_iterate` (iterates converging to y implies y is fixed), `isClosed_fixedPoints` (fixed point set is closed in T2 spaces) |

## Subdirectories

*(none)*

## Search Tags

fixed-points isFixedPt fixedPoints self-map iteration semiconjugacy permutation topology closed-set convergence prufer-subgroup pointwise-action commuting-maps bijection
