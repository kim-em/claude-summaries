---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/CStarAlgebra
generated: 2025-12-04T14:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 17
subdirs_count: 4
---

# CStarAlgebra

## Overview

The `CStarAlgebra/` directory contains the formalization of C⋆-algebra theory. C⋆-algebras are Banach ⋆-algebras over ℂ (or more generally a densely normed field) satisfying the C⋆-identity `‖x⋆ * x‖ = ‖x‖²`. This directory includes basic definitions, classes for unital and non-unital C⋆-algebras, spectral theory, the Gelfand duality theorem (contravariant equivalence between compact Hausdorff spaces and commutative unital C⋆-algebras), multiplier algebras, continuous functional calculus, and various structural results. The formalization covers both commutative and noncommutative C⋆-algebras, approximate units, positive and completely positive maps, and connections to operator theory via matrices.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines normed star groups and rings; establishes fundamental properties of the `star` involution being isometric; provides foundational structure for C⋆-rings |
| Classes.lean | Defines the main C⋆-algebra type classes: `NonUnitalCStarAlgebra`, `NonUnitalCommCStarAlgebra`, `CStarAlgebra`, and `CommCStarAlgebra` (requires complex imports) |
| Spectrum.lean | Spectral properties in C⋆-algebras: spectrum of unitary elements is in unit circle, spectrum of selfadjoint elements is real, spectral radius equals norm for selfadjoint/normal elements, and spectral permanence |
| GelfandDuality.lean | The Gelfand transform and Gelfand duality theorem; establishes the contravariant equivalence between compact Hausdorff spaces and commutative unital C⋆-algebras via functors `F(X) = C(X,ℂ)` and `G(A) = characterSpace ℂ A` |
| Multiplier.lean | Multiplier algebra `𝓜(𝕜, A)` defined as double centralizers (pairs of continuous linear maps `L R : A →L[𝕜] A` satisfying `R x * y = x * L y`); corresponds to non-commutative Stone–Čech compactification |
| Unitization.lean | Shows the minimal unitization of a C⋆-algebra is also a C⋆-algebra; proves every C⋆-algebra is a regular normed algebra and that right multiplication is isometric |
| ApproximateUnit.lean | Nonnegative contractions in a (possibly non-unital) C⋆-algebra form a directed approximate unit; uses continuous functional calculus with functions `1 - (1 + x)⁻¹` and `x * (1 - x)⁻¹` |
| CStarMatrix.lean | Type copy `CStarMatrix m n A` for matrices with entries in a C⋆-algebra; operator norm makes `CStarMatrix n n A` a C⋆-algebra |
| Matrix.lean | Transports operator norm on `EuclideanSpace 𝕜 n →L[𝕜] EuclideanSpace 𝕜 m` to `Matrix m n 𝕜`; provides scoped normed ring instance ensuring matrices form a C⋆-ring |
| Hom.lean | Properties of C⋆-algebra homomorphisms; proves non-unital star algebra monomorphisms of complex C⋆-algebras are isometric and preserve spectra |
| CompletelyPositiveMap.lean | Completely positive (CP) maps: linear maps `φ : A₁ →ₗ[ℂ] A₂` where applying φ entrywise to k×k matrices is positive for all k; shows non-unital star algebra homomorphisms are CP |
| PositiveLinearMap.lean | Positive linear maps in C⋆-algebras; proves positive maps are bounded and therefore continuous on non-unital C⋆-algebras |
| Projection.lean | Projections in C⋆-algebras; shows idempotent elements are self-adjoint iff normal, characterizing star projections |
| Exponential.lean | Exponential map in C⋆-algebras |
| ContinuousLinearMap.lean | Import file for continuous linear maps in C⋆-algebras |
| ContinuousMap.lean | Import file for continuous maps in C⋆-algebras |
| lpSpace.lean | Connections between C⋆-algebras and Lp spaces |

## Subdirectories

- [x] `ContinuousFunctionalCalculus/` - Continuous functional calculus for C⋆-algebras (applying continuous functions to operators); includes basic theory, instances, integral formulation, isometric properties, order properties, restrictions, uniqueness, and separate unital/non-unital treatments (complete)
- [ ] `Module/` - Module theory for C⋆-algebras; constructions and definitions for modules over C⋆-algebras, type synonyms (pending)
- [ ] `SpecialFunctions/` - Special functions in C⋆-algebras using continuous functional calculus; positive part function (pending)
- [ ] `Unitary/` - Theory of unitary elements in C⋆-algebras; connectedness properties of unitary group and span of unitaries (pending)

## Search Tags

cstar-algebras banach-star-algebras normed-star-groups functional-analysis operator-algebras gelfand-duality spectral-theory spectrum unitization multiplier-algebra approximate-units continuous-functional-calculus positive-maps completely-positive-maps star-homomorphisms unitary-elements projections selfadjoint-elements normal-elements commutative-cstar-algebras noncommutative-algebras character-space matrix-algebras operator-norm stone-cech-compactification
