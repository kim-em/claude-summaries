---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/QuadraticAlgebra
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# QuadraticAlgebra

## Overview

Quadratic algebras over commutative rings, representing extensions of the form `R[X]/(X²-bX-a)` where `i² = a + bi`. The implementation provides a structure `QuadraticAlgebra R a b` with real and imaginary parts, equipped with complete algebraic infrastructure (ring/field structures, star involution, norm map), free module structure over R with rank 2, and connections to linear algebra via determinants. This generalizes both complex numbers and quaternions as special cases of quadratic field extensions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `QuadraticAlgebra R a b` as a structure with `re` and `im` fields satisfying `i² = a + bi`, with equivalence to `R × R`, complete algebraic hierarchy (zero/one/add/neg/mul/smul instances), ring/algebra structures for commutative semirings/rings, module structure proving it's a free rank-2 module with explicit basis `[1, ω]`, and divisibility theory |
| Basic.lean | Star involution `star ⟨x, y⟩ = ⟨x + by, -y⟩` implementing `StarRing` typeclass, norm map `z ↦ z.re² + b·z.re·z.im - a·z.im²` as a `MonoidHom`, unit characterization `IsUnit z ↔ IsUnit (norm z)`, unitary elements as norm kernel, zero-divisor theory `z.norm ∈ R⁰ ↔ z ∈ (QuadraticAlgebra R a b)⁰`, and field instance when R is a field and no `r : R` satisfies `r² = a + br` (irreducibility condition) |
| NormDeterminant.lean | Proves that `norm z` equals the determinant of the left-multiplication endomorphism `x ↦ z * x`, connecting the algebraic norm to linear algebra via `det_toLinearMap_eq_norm` |

## Subdirectories

None.

## Search Tags

quadratic-algebra quadratic-extension field-extension algebra star-ring norm determinant free-module rank-2 commutative-ring irreducible polynomial-quotient
