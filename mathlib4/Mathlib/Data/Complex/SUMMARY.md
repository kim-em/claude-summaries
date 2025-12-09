---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Complex
generated: 2025-12-08T23:30:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 9
subdirs_count: 0
---

# Complex

## Overview

This directory contains the basic definition and core algebraic properties of complex numbers (ℂ) in mathlib4. Complex numbers are modeled as pairs of real numbers (ℝ²) with the standard field structure, including addition, multiplication, conjugation, norm squared, and inversion. The main implementation is in `Basic.lean`, which establishes that ℂ forms a field of characteristic zero. Several deprecated module files provide backward-compatible imports redirecting to their new locations in the `Analysis/` and `LinearAlgebra/` hierarchies.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of complex numbers as `structure Complex` with real and imaginary parts; establishes field structure, imaginary unit `I`, conjugation, norm squared, inversion, and characteristic zero; includes arithmetic operations, casting from reals, and equivalence with ℝ × ℝ (832 lines) |
| BigOperators.lean | Finite sums and products over complex numbers; proves that `ofReal`, `re`, and `im` commute with sums, products, expectations, and balance operations over finsets |
| Cardinality.lean | Deprecated module redirecting to `Mathlib.Analysis.Complex.Cardinality` (since 2025-08-26) |
| Exponential.lean | Deprecated module redirecting to `Mathlib.Analysis.Complex.Exponential` (since 2025-08-26) |
| ExponentialBounds.lean | Deprecated module redirecting to `Mathlib.Analysis.Complex.ExponentialBounds` (since 2025-08-26) |
| FiniteDimensional.lean | Deprecated module redirecting to `Mathlib.LinearAlgebra.Complex.FiniteDimensional` (since 2025-08-26) |
| Norm.lean | Deprecated module redirecting to `Mathlib.Analysis.Complex.Norm` (since 2025-08-26) |
| Order.lean | Deprecated module redirecting to `Mathlib.Analysis.Complex.Order` (since 2025-08-26) |
| Trigonometric.lean | Deprecated module redirecting to `Mathlib.Analysis.Complex.Trigonometric` (since 2025-08-26) |

## Search Tags

complex-numbers field-structure imaginary-unit conjugation norm-squared arithmetic real-imaginary-parts type-theory algebraic-structures characteristic-zero deprecated-modules module-reorganization
