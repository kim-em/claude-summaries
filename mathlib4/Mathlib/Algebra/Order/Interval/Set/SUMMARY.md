---
source_path: /Users/kim/projects/lean/lean4-2/downstream_releases/mathlib4/Mathlib/Algebra/Order/Interval/Set
generated: 2025-12-01T22:00:00Z
git_sha: 8630639169c28647dbae9f5b0132c77dcbfe2281
git_branch: bump_to_v4.26.0-rc2
status: complete
files_count: 4
subdirs_count: 0
---

# Set

## Overview

The `Set/` directory provides algebraic properties and operations on set-based intervals (`Set.Ixx`) for ordered algebraic structures. It defines group and monoid operations on intervals (proving membership characterizations for addition, subtraction, multiplication, and inversion), algebraic instances for unit intervals [0,1] (monoid/semigroup structures for Icc, Ico, Ioc, Ioo), bijective translation of intervals under addition, pairwise disjointness of translated/scaled intervals, and successor-predecessor relations for intervals in additive orders.

## Key Files

| File | Purpose |
|------|---------|
| Group.lean | Group and monoid operations on set intervals: proves membership characterizations (`inv_mem_Ixx_iff`, `add_mem_Ixx_iff`, `sub_mem_Ixx_iff`) for intervals under ordered comm groups/additive comm groups, absolute value interval membership, and pairwise disjointness lemmas for translated/scaled intervals (zpow, zsmul, integer casts) |
| Instances.lean | Algebraic instances for unit intervals [0,1]: defines Zero/One/Mul/Pow instances and proves Icc has CancelCommMonoidWithZero, Ico has CommSemigroup, Ioc has CancelCommMonoid, Ioo has CommSemigroup; includes one-minus-membership lemmas and inequalities for unit interval elements |
| Monoid.lean | Images of intervals under translation: proves that addition maps (`· + d`, `d + ·`) are bijections on all interval types (Ici, Ioi, Icc, Ico, Ioc, Ioo) for ordered cancel add monoids with ExistsAddOfLE, enabling interval translation in non-group settings like ℕ and ℝ≥0 |
| SuccPred.lean | Set intervals in additive successor-predecessor orders: relates intervals via `a+1` and `b-1` transformations (e.g., `Ico (a+1) b = Ioo a b`, `Icc (a+1) (b-1) = Ioo a b`), proves insertion lemmas for extending intervals by endpoints, covers both SuccAddOrder and PredSubOrder with/without max/min elements |

## Subdirectories

(none)

## Search Tags

set-intervals group-operations monoid-operations interval-membership unit-intervals interval-translation ordered-groups ordered-monoids successor-predecessor interval-bijections pairwise-disjoint algebraic-instances interval-insertion cancel-monoid comm-monoid zero-one-intervals
