---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Rat
generated: 2025-12-11T12:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: preliminary
files_count: 10
subdirs_count: 2
---

# Rat

## Overview

The `Rat/` directory contains the foundational implementation of rational numbers (ℚ) in mathlib4. It defines the algebraic structure (integral domain, additive/multiplicative groups), arithmetic operations (addition, multiplication, division, powers), and key properties of rationals including floor/ceiling functions, square roots, encoding/denumerability, and star-ordered ring structure. The implementation builds on Lean's core `Rat` type, providing the `divInt` (/.`) notation for constructing rationals from integers and proving fundamental lemmas about numerator/denominator manipulation.

## Key Files

| File | Purpose |
|------|---------|
| Init.lean | Basic definitions: `ℚ` notation, `NNRat` (non-negative rationals ℚ≥0), and `NNRatCast` typeclass for canonical homomorphisms |
| Defs.lean | Core algebraic structure: `AddCommGroup`, `CommMonoid` instances; `divInt` notation (n /. d); lemmas about numerator/denominator; injectivity of casts from ℤ and ℕ |
| Lemmas.lean | Further arithmetic lemmas: divisibility of num/den, operations on denominators under addition/subtraction/multiplication, `pnatDen` (denominator as ℕ+), coprimality properties |
| Floor.lean | `FloorRing` instance for ℚ; floor/ceiling/round/fract operations; `norm_num` extensions for computing floor/ceil/round on rational literals |
| BigOperators.lean | Casting lemmas for sums/products: `cast_sum`, `cast_prod`, `cast_list_sum`, `cast_multiset_sum` over division rings with characteristic zero |
| Cardinal.lean | Proves `#ℚ = ℵ₀` (cardinality of rationals is countably infinite) |
| Denumerable.lean | `Denumerable` instance for ℚ (bijection with ℕ) |
| Encodable.lean | `Encodable` instance for ℚ (and thus `Countable`) via equivalence with Σ-type of numerator and coprime positive denominator |
| Sqrt.lean | `Rat.sqrt` function (integer square root of numerator over natural square root of denominator); `DecidablePred IsSquare` instance |
| Star.lean | `StarOrderedRing` instances for ℚ and ℚ≥0; proves every non-negative rational is a sum of squares |

## Subdirectories

- [x] `Cast/` - Casting operations between ℚ and other types (CharZero, order-preserving casts, scientific notation)
- [x] `NatSqrt/` - Natural number square root approximations for rationals

## Search Tags

rational-numbers rationals ℚ divInt floor ceiling round fract encodable denumerable countable cardinality aleph-zero square-root star-ordered-ring sum-of-squares bigoperators cast
