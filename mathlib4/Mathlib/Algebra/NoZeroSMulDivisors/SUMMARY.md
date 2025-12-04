---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/NoZeroSMulDivisors
generated: 2025-12-04T08:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# NoZeroSMulDivisors

## Overview

The `NoZeroSMulDivisors/` directory defines the `NoZeroSMulDivisors R M` typeclass, which states that scalar multiplication `c • x = 0` if and only if either the scalar `c` or the vector `x` is zero. This is a heterogeneous generalization of `NoZeroDivisors` to scalar actions and serves as a characteristic-independent notion of torsion-freeness for modules. The directory provides the core definition, fundamental lemmas about vanishing scalar products (especially for modules over division rings), connections to characteristic zero and additive torsion-freeness, and instances for product and function types.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `NoZeroSMulDivisors` typeclass with fundamental characterization `smul_eq_zero : c • x = 0 ↔ c = 0 ∨ x = 0`, pullback along injective functions, connection to `NoZeroDivisors`, equivalences with `IsAddTorsionFree` for ℕ and ℤ scalars, and TODO note about replacing with `Module.IsTorsionFree` |
| Basic.lean | Advanced theory: characteristic zero propagation from modules to rings, injectivity of scalar multiplication (`smul_right_injective`, `smul_left_injective`), proof that characteristic zero is necessary for nontrivial torsion-free modules, canonical `NoZeroSMulDivisors` instance for `GroupWithZero` actions (covering division semirings like ℝ≥0 and ℚ≥0) |
| Pi.lean | `NoZeroSMulDivisors` instance for dependent function types `(i : I) → f i` and non-dependent functions `ι → β`, proving that scalar multiplication is zero-free componentwise |
| Prod.lean | `NoZeroSMulDivisors` instance for binary products `M × N`, showing the property holds coordinatewise |

## Subdirectories

*(No subdirectories)*

## Search Tags

no-zero-smul-divisors scalar-multiplication torsion-free modules characteristic-zero smul-injective pi-instances product-instances group-with-zero division-semiring
