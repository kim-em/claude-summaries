---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/NNRat
generated: 2025-12-09T10:30:38Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 5
subdirs_count: 0
---

# NNRat

## Overview

The `NNRat/` directory implements non-negative rational numbers (ℚ≥0), defined as a subtype of `Rat` with the constraint that the value is non-negative. It provides the foundational definitions, algebraic operations, order structures, and conversion functions between `ℚ≥0` and `ℚ`. The implementation includes basic arithmetic (addition, multiplication, subtraction as truncated difference), ordering, floor/ceiling operations, and integration with big operators (sums and products). These files establish ℚ≥0 as a canonically ordered commutative semiring with characteristic zero.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions and basic algebraic structure for `NNRat` (ℚ≥0); defines nonnegative rationals as subtype `{q : ℚ // 0 ≤ q}`, provides coercion, injection lemmas, `Rat.toNNRat` conversion, arithmetic operations, numerator/denominator access, `divNat` for constructing rationals from natural numbers, and establishes instances for `CommSemiring`, `LinearOrder`, `CharZero`, and `OrderBot` |
| Lemmas.lean | Field and action structures that depend on more advanced imports; includes `coe_indicator` for set indicators, inverse and division operations (`toNNRat_inv`, `toNNRat_div`), recursor for pattern matching on numerators/denominators, and formulas for multiplication's effect on numerators and denominators |
| BigOperators.lean | Casting lemmas for operations involving sums and products over lists, multisets, and finsets; proves that casting distributes over `∑` and `∏`, and provides `toNNRat_sum_of_nonneg` and `toNNRat_prod_of_nonneg` for converting rational sums/products to nonnegative rationals when all terms are nonnegative |
| Floor.lean | Floor and ceiling operations for ℚ≥0; defines `FloorSemiring` instance, relates `⌊·⌋₊` and `⌈·⌉₊` to the corresponding operations on ℚ, proves casting compatibility with floor/ceiling in other semifields and fields, and includes `norm_num` meta extension for evaluating `Nat.ceil` |
| Order.lean | Bundled ordered algebra instances; establishes `IsStrictOrderedRing`, `OrderedSub`, and `CanonicallyOrderedAdd` instances by lifting from the `Nonneg` construction |

## Subdirectories

*(No subdirectories)*

## Search Tags

nonnegative-rationals nnrat coercion subtype semiring linear-order floor ceiling toNNRat divNat numerator denominator big-operators sums products characteristic-zero ordered-structures
