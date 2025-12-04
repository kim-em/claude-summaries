---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/AbsoluteValue
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# AbsoluteValue

## Overview

This directory formalizes the theory of equivalence of real-valued absolute values on fields. Two absolute values are considered equivalent if they preserve the same ordering (i.e., `v x ≤ v y ↔ w x ≤ w y`), which for real absolute values is equivalent to the existence of a positive real constant `c` such that `v x ^ c = w x` for all `x`. The formalization includes the algebraic characterization of equivalence, the construction of divergent points that distinguish inequivalent absolute values (including the generalization to finite families of pairwise inequivalent absolute values), and the topological characterization showing that two real absolute values are equivalent if and only if they induce homeomorphic completions.

## Key Files

| File | Purpose |
|------|---------|
| Equivalence.lean | Defines equivalence of absolute values via order preservation; proves equivalence relation properties (reflexivity, symmetry, transitivity); shows equivalence of trivial absolute value characterization; establishes existence of divergent points for inequivalent absolute values (elements where one absolute value is < 1 while the other is ≥ 1); generalizes to finite families of pairwise inequivalent absolute values via strong induction; proves real absolute values are equivalent iff related by power `v x ^ c = w x` for positive constant `c`; shows equivalence is characterized by induced topologies being homeomorphic via `WithAbs.equivWithAbs` |

## Subdirectories

None - this is a leaf directory.

## Search Tags

absolute-value equivalence field real-valued ordering divergent-points homeomorphism topology nontrivial archimedean linear-order power-relation rpow logarithm WithAbs pairwise-inequivalent finite-families strong-induction
