---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Module/LinearMap
generated: 2025-12-01T18:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 8
subdirs_count: 0
---

# LinearMap

## Overview

The `LinearMap/` directory defines linear maps (module homomorphisms) and semilinear maps between modules, which are the fundamental structure-preserving maps in module theory. A semilinear map `f : M →ₛₗ[σ] M₂` between an R-module M and an S-module M₂ satisfies `f(x + y) = f(x) + f(y)` and `f(c • x) = σ(c) • f(x)` for a ring homomorphism `σ : R →+* S`. Linear maps are the special case where `σ = RingHom.id`. The directory includes the core `LinearMap` structure definition with its basic algebraic instances (addition, scalar multiplication, composition), specialized results for linear endomorphisms (which form a ring under composition), linear functionals on division rings, characteristic polynomials of linear families of endomorphisms, rational linear maps, star-linear maps, and proofs that addition/subtraction are linear maps from product spaces.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `LinearMap σ M M₂` structure (extends `AddHom` and `MulActionHom`), `IsLinearMap` predicate, notations `M →ₛₗ[σ] M₂` (semilinear) and `M →ₗ[R] M₂` (linear), basic instances for additive structure and scalar actions |
| Basic.lean | Extended linear map theory: `ltoFun` (coerce linear map to function linearly), domain-acted scalar multiplication on linear maps (`S'ᵈᵐᵃ` action), `DistribMulAction` and `Module` instances with commutativity constraints, `NoZeroSMulDivisors` for linear maps |
| End.lean | Linear endomorphisms `Module.End R M = M →ₗ[R] M`: monoid structure from composition, semiring/ring instances (multiplication is composition, addition is pointwise), natural number and integer casts as scalar multiples of identity |
| DivisionRing.lean | Linear functionals on division rings: `surjective_iff_ne_zero` (functional is surjective iff nonzero), `range_smulRight_apply` (range of `f.smulRight x` equals span of `{x}` for nonzero functional `f`) |
| Polynomial.lean | Characteristic polynomials of linear families: `Matrix.toMvPolynomial` (matrix to multivariate polynomial), `LinearMap.polyCharpoly` (multivariate polynomial evaluating to characteristic polynomial of `φ x`), `polyCharpoly_coeff_isHomogeneous` (coefficients are homogeneous), `nilRank` and `IsNilRegular` for nil-regularity theory used in Lie algebras |
| Prod.lean | Addition and subtraction as linear maps from product spaces: `IsLinearMap.isLinearMap_add` proves `(x, y) ↦ x + y` is linear, `isLinearMap_sub` for subtraction |
| Rat.lean | Rational linear maps: `AddMonoidHom.toRatLinearMap` reinterprets additive homomorphisms between ℚ-modules as ℚ-linear maps using `map_rat_smul`, with injectivity proof |
| Star.lean | Star-linear map notation: `M →ₗ⋆[R] N` for conjugate-linear maps (semilinear maps via `starRingEnd R`), `M ≃ₗ⋆[R] M₂` for star-linear equivalences |

## Subdirectories

(none)

## Search Tags

linear-map semilinear-map module-homomorphism endomorphism characteristic-polynomial linear-functional division-ring star-linear conjugate-linear nil-rank nil-regular polyCharpoly Lie-theory rational-linear-map product-space composition ring-structure
