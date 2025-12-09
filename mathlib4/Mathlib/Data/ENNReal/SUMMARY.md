---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/ENNReal
generated: 2025-12-09T22:18:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 9
subdirs_count: 0
---

# ENNReal

## Overview

The `Data/ENNReal/` directory contains the complete theory of extended non-negative real numbers (`ℝ≥0∞`), defined as `WithTop ℝ≥0` to represent the interval `[0, ∞]`. This type is fundamental to measure theory (as the codomain of measures) and extended metric spaces (for extended distance functions). The directory provides the full algebraic structure (addition, multiplication, subtraction, inversion, division, powers), order theory, lattice operations, conversions to/from real numbers and non-negative reals, and big operators (sums, products). The code establishes `ℝ≥0∞` as a canonically ordered commutative semiring with complete linear order and proper handling of infinity in all operations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `ENNReal := WithTop ℝ≥0` with notation `ℝ≥0∞`; establishes fundamental algebraic instances (semiring, ordered structures, lattice operations), coercions from `ℝ≥0`, conversion functions (`toNNReal`, `toReal`, `ofReal`), and basic order properties; proves many theorems about interactions with `∞` |
| Operations.lean | Properties of addition, multiplication, subtraction, and natural powers; proves monotonicity, cancellation, strictness properties; establishes how these operations interact with `∞` and with order relations; includes theorems about suprema/infima of operations |
| Inv.lean | Theory of inversion and division on `ℝ≥0∞`; defines `a⁻¹ = sInf {b \| 1 ≤ a * b}` with special cases `0⁻¹ = ∞` and `∞⁻¹ = 0`; proves `DivInvOneMonoid` instance, cancellation properties, order isomorphisms involving inversion, integer powers (`zpow`), and unit interval birational mappings |
| Real.lean | Conversions between `ℝ≥0∞` and `ℝ`; properties of `toReal`, `ofReal`, and their interactions with algebraic operations (addition, multiplication, powers); monotonicity and comparison theorems; special results like trichotomy and dichotomy lemmas often used in `Lp` space theory; includes `positivity` tactic extension for `ofReal` |
| BigOperators.lean | Finite sums and products on `ℝ≥0∞`; proves that sums/products of finite values remain finite, conversion between `ℝ≥0∞` and `ℝ≥0` sums, interaction of products with inversion/division, and suprema of finite sums; establishes when finite operations equal `∞` |
| Action.lean | Scalar multiplication on `ℝ≥0∞`; shows that `MulAction`, `DistribMulAction`, `Module`, and `Algebra` structures over `ℝ≥0∞` restrict to `ℝ≥0`; proves strict monotonicity and positivity properties of scalar multiplication; includes conversion lemmas for `toNNReal` and `toReal` under scalar multiplication |
| Holder.lean | Hölder's inequality for extended non-negative reals; proves the fundamental inequality for conjugate exponents used extensively in analysis and `Lp` space theory |
| Lemmas.lean | Miscellaneous auxiliary lemmas requiring additional imports; includes indicator function coercion and finset supremum properties; split off from `Basic.lean` to reduce import dependencies |
| Order.lean | Deprecated module (since 2025-04-13) that now simply re-exports `Operations.lean`; kept for backward compatibility |

## Subdirectories

None.

## Search Tags

extended-nonnegative-reals ennreal measure-theory metric-spaces infinity lattice-operations supremum infimum addition multiplication inversion division powers conversions toReal ofReal toNNReal big-operators holder-inequality scalar-multiplication canonically-ordered-semiring complete-linear-order
