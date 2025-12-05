---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Ring
generated: 2025-12-05T08:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 8
subdirs_count: 0
---

# Ring

## Overview

The `Ring/` directory provides the core theory of normed rings in mathlib4. It defines the fundamental typeclasses `NonUnitalSeminormedRing`, `SeminormedRing`, `NonUnitalNormedRing`, and `NormedRing`, which combine ring structure with norms satisfying the submultiplicative inequality `‖x * y‖ ≤ ‖x‖ * ‖y‖`. The directory includes theory for units in complete normed rings (invertibility and openness), infinite sums and the Cauchy product formula, integer and finite-order element norms, ultrametric norms, and the `WithAbs` type synonym for handling multiple absolute value instances on the same ring.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines core normed ring typeclasses (`NonUnitalSeminormedRing`, `SeminormedRing`, `NonUnitalNormedRing`, `NormedRing`, and commutative variants); provides submultiplicative norm axiom `‖x * y‖ ≤ ‖x‖ * ‖y‖`; includes semiring instance constructions and proof helper lemmas |
| Lemmas.lean | Proves theorems about normed rings: tendsto lemmas for multiplication with bounded sequences, Pi type instances (product of finitely many normed rings with sup norm), `RingHomIsometric` properties, and power functions with cobounded filters |
| Units.lean | Theory of units (invertible elements) in complete normed rings: constructs `Units.add` and `Units.ofNearby` showing perturbations of units are units; proves `Units.isOpen` (units form open subset); derives asymptotic properties of `Ring.inverse` including `NormedRing.inverse_add` and norm estimates |
| InfiniteSum.lean | Multiplying infinite sums in normed rings: proves summability of products `(∑' x, f x) * (∑' y, g y)` from summability of norms; establishes `tsum_mul_tsum_of_summable_norm` and Cauchy product formula `tsum_mul_tsum_eq_tsum_sum_antidiagonal_of_summable_norm` for ℕ-indexed families |
| Ultra.lean | Ultrametric norm behavior in normed rings with `NormOneClass` (where `‖1‖ = 1`): proves `norm_natCast_le_one` and `norm_intCast_le_one` showing natural/integer casts have norm ≤ 1; uses ultrametric property `‖x + 1‖ ≤ max ‖x‖ 1` |
| Int.lean | Norm properties of integers as normed ring: proves `Int.nnnorm_coe_units` (units ±1 have norm 1), `Int.nnnorm_natCast` (norm of natural cast equals the natural number), and lemmas relating `toNat` with norms |
| Finite.lean | Finite order elements in normed rings: proves `IsOfFinOrder.norm_eq_one` (elements with `xⁿ = 1` have `‖x‖ = 1` in rings with `NormMulClass` and `NormOneClass`); includes `AddChar.norm_apply` showing additive character values on finite monoids have norm 1 |
| WithAbs.lean | `WithAbs v` type synonym for a semiring depending on an absolute value; allows type inference to handle multiple absolute value instances on same ring; provides `WithAbs.equiv` (canonical equivalence to underlying ring), `normedRing` instance from absolute values, and `AbsoluteValue.LiesOver` for extension of absolute values |

## Subdirectories

(none)

## Search Tags

normed-rings seminormed-rings submultiplicative-norm ring-norm units-open invertible-elements complete-normed-rings banach-rings infinite-sums cauchy-product tsum-multiplication ultrametric-rings nonarchimedean integer-norms finite-order-elements norm-one-class absolute-values with-abs ring-homomorphisms isometric-homomorphisms geometric-series inverse-function
