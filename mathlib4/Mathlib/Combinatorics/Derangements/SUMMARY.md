---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Derangements
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# Derangements

## Overview

The `Derangements/` directory formalizes the theory of derangements—permutations without fixed points. It defines derangements on arbitrary types, proves recursive decomposition equivalences involving `Option α`, and establishes cardinality results for finite types. The directory culminates in a proof that the probability of a random permutation being a derangement approaches 1/e as the set size grows, connecting discrete combinatorics to analysis via exponential series.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of derangements as `{ f : Perm α \| ∀ x, f x ≠ x }`; proves equivalences between derangements on `Option α` and sigma-types of permutations with at most one fixed point, establishing recursive structure via `derangementsRecursionEquiv` |
| Finite.lean | Cardinality results for derangements on finite types: proves `card (derangements α)` depends only on `card α`, defines `numDerangements n` recursively as `(n+1)*(D(n) + D(n+1))`, and establishes summation formula in terms of ascending factorials |
| Exponential.lean | Asymptotic analysis: proves `numDerangements_tendsto_inv_e` showing that `D(n)/n!` converges to `exp(-1) = 1/e`, connecting the derangement recurrence to the power series for exponential functions |

## Subdirectories

*(No subdirectories)*

## Search Tags

derangements fixed-points permutations combinatorics enumeration factorial exponential-series asymptotic-analysis recursive-decomposition option-type sigma-type cardinality fintype probability-limit ascending-factorial
