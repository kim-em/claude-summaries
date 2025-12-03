---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/BigOperators/Group/Multiset
generated: 2025-12-01T17:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Multiset

## Overview

The `Multiset/` directory defines products and sums over multisets (unordered collections with multiplicity). It provides `Multiset.prod` and `Multiset.sum`, which serve as the intermediate layer between `List.prod`/`List.sum` (ordered sequences) and `Finset.prod`/`Finset.sum` (finite sets). The implementation leverages the fact that multisets are quotients of lists by permutation equivalence, defining `Multiset.prod` via `foldr` and proving it respects the equivalence relation. This layer is crucial for defining finite sums and products since it handles the transition from ordered (lists) to unordered (finsets) aggregation.

## Key Files

| File | Purpose |
|------|---------|
| `Defs.lean` | Core definitions of `Multiset.prod` and `Multiset.sum` via `foldr`, with fundamental properties like `prod_cons`, `prod_singleton`, `prod_replicate`, and basic induction principles |
| `Basic.lean` | Extensive library of theorems for multiset products and sums, including homomorphism properties (`prod_hom`, `prod_hom₂`), interaction with operations (`prod_add`, `prod_map_mul`, `prod_map_inv`), modular arithmetic, and specialized results for division monoids and ordered subtraction |

## Subdirectories

*(No subdirectories)*

## Search Tags

multiset big-operators product sum commutative-monoid quotient foldr homomorphism list-to-finset unordered-collection multiplicity algebraic-structures
