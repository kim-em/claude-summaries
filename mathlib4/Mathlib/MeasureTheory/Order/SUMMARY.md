---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Order
generated: 2026-01-25T22:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 2
subdirs_count: 1
---

# Order

## Overview

The `Order/` directory provides measure-theoretic results for ordered structures, combining order theory with measurability. It defines typeclasses for measurability of lattice operations (supremum and infimum), proves that order-connected sets in ℝⁿ have null frontiers (and are thus null-measurable), and extends these results to groups with lattice structure. The core contributions include the `MeasurableSup` and `MeasurableInf` typeclass hierarchies with dot-style lemmas, and the surprising result that any order-connected set in finite-dimensional Euclidean space is null-measurable despite not generally being Borel measurable.

## Key Files

| File | Purpose |
|------|---------|
| Lattice.lean | Typeclasses for measurability of lattice operations: defines `MeasurableSup`, `MeasurableInf` (for unary operations like `(c ⊔ ·)`) and `MeasurableSup₂`, `MeasurableInf₂` (for binary operations `uncurry (· ⊔ ·)`), with dot-style lemmas for `Measurable` and `AEMeasurable`, instances for `OrderDual`, and measurability results for finset suprema |
| UpperLower.lean | Proves order-connected sets in ℝⁿ are null-measurable: shows that upper sets, lower sets, and order-connected sets all have null frontiers using the Lebesgue density theorem and Besicovitch covering, proves antichains have measure zero, works with the ∞-metric (pointwise max norm) on `ι → ℝ` |

## Subdirectories

- [x] `Group/` - Measurability results for groups with lattice structure (positive/negative parts, multiplicative absolute value)

## Search Tags

measurable lattice sup inf order-connected upper-set lower-set null-frontier null-measurable lebesgue-density besicovitch antichain measurable-sup measurable-inf pointwise-order euclidean-space
