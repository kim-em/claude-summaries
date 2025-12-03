---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Positive
generated: 2025-12-01T21:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Positive

## Overview

The `Positive/` directory provides algebraic structure instances for the positive subtype `{x : R // 0 < x}`, enabling positive elements to be treated as standalone algebraic objects. It defines additive structures (semigroups with cancellation and monotonicity), multiplicative structures (monoids, ordered monoids, cancellative monoids), and for fields, shows that positive elements form a commutative group under multiplication with integer powers. The approach mirrors the nonnegative subtype development but focuses on strictly positive elements, requiring weaker typeclass assumptions where possible.

## Key Files

| File | Purpose |
|------|---------|
| Ring.lean | Core algebraic instances for positive subtypes: `Add`, `AddSemigroup`, `AddCommSemigroup` with cancellation variants, additive monotonicity/reflection instances, `Mul`, `Monoid`, `CommMonoid`, `Distrib`, and ordered monoid structures (`IsOrderedMonoid`, `IsOrderedCancelMonoid`) for semirings and commutative semirings |
| Field.lean | Commutative group structure on positive elements of linear ordered fields: defines `Inv` instance with `x⁻¹ = (x⁻¹, inv_pos)`, integer power `Pow ℤ` instance, and proves `CommGroup` structure via `inv_mul_cancel` |

## Subdirectories

None.

## Search Tags

positive-elements positive-subtype ordered-algebra strictly-positive algebraic-structures additive-semigroup commutative-monoid ordered-monoid field-group integer-powers inverse-positive cancellation-semigroup monotone-addition
