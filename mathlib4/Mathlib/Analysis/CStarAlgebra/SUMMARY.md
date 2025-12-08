---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/CStarAlgebra
generated: 2025-12-04T18:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 17
subdirs_count: 4
---

# CStarAlgebra

## Overview

The `CStarAlgebra/` directory contains a comprehensive formalization of C⋆-algebra theory and related structures in functional analysis. C⋆-algebras are Banach ⋆-algebras over ℂ (or more generally a densely normed field) satisfying the C⋆-identity `‖x⋆ * x‖ = ‖x‖²`. This directory provides the foundational definitions, type classes for both unital and non-unital variants, spectral theory results, and deep structural theorems.

The formalization includes several major theoretical components: (1) **Continuous functional calculus** enables applying continuous functions to operators, providing both unital (`cfc`) and non-unital (`cfcₙ`) APIs with support for complex, real, and nonnegative scalars, complete with isometric properties, continuity theorems, and spectral mapping results. (2) **Gelfand duality** establishes the contravariant equivalence between compact Hausdorff spaces and commutative unital C⋆-algebras via the Gelfand transform. (3) **Hilbert C⋆-modules** generalize Hilbert spaces to modules with A-valued inner products, including constructions for products, pi-types, and inner product spaces. (4) **Unitary theory** proves the unitary group is locally path connected and that unitaries span the entire algebra. (5) **Structural results** on positive/negative part decompositions, approximate units, multiplier algebras, and spectral properties.

The theory covers both commutative and noncommutative C⋆-algebras, with particular attention to homomorphisms (which are automatically isometric), completely positive maps, projections, exponentials, and connections to matrix algebras with operator norms.

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

- [x] `ContinuousFunctionalCalculus/` - Continuous functional calculus for C⋆-algebras (applying continuous functions to operators); includes basic theory, instances, integral formulation, isometric properties, order properties, restrictions, uniqueness, and separate unital/non-unital treatments
- [x] `Module/` - Hilbert C⋆-modules with A-valued inner products; main class definition, Cauchy-Schwarz inequality, constructions (products, pi-types, C⋆-algebras as self-modules, inner product spaces), and WithCStarModule type synonym for norm management
- [x] `SpecialFunctions/` - C⋆-algebraic facts about positive and negative parts of elements; spanning by nonnegative contractions and decomposition results
- [x] `Unitary/` - Theory of unitary elements in C⋆-algebras; connectedness properties of unitary group and span of unitaries

## Search Tags

cstar-algebras banach-star-algebras normed-star-groups functional-analysis operator-algebras gelfand-duality spectral-theory spectrum unitization multiplier-algebra approximate-units continuous-functional-calculus positive-maps completely-positive-maps star-homomorphisms unitary-elements projections selfadjoint-elements normal-elements commutative-cstar-algebras noncommutative-algebras character-space matrix-algebras operator-norm stone-cech-compactification
