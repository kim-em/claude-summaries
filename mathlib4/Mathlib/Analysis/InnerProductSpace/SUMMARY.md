---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/InnerProductSpace
generated: 2025-12-05T10:27:15Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 41
subdirs_count: 2
---

# InnerProductSpace

## Overview

This directory contains the comprehensive formalization of inner product spaces and Hilbert spaces in Lean. It defines the fundamental structure of inner product spaces (vector spaces with inner products generalizing the dot product), proves core theorems like the Cauchy-Schwarz inequality and polarization identity, and develops the complete theory of orthogonality, projections, adjoints, and spectral theory for self-adjoint operators. The implementation handles both real and complex inner product spaces uniformly through the `RCLike` typeclass, with the convention that inner products are conjugate-linear in the first argument and linear in the second. The directory includes specialized subdirectories for orthogonal projection theory (existence theorems, reflection isometries, finite-dimensional results including Cartan-Dieudonné theorem) and harmonic functions (connecting inner product spaces with complex analysis by proving that complex-analytic functions are harmonic).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of inner product spaces; defines the `InnerProductSpace` typeclass, inner product notation `⟪·, ·⟫`, and the `InnerProductSpace.Core` structure for constructing normed spaces from inner products |
| Basic.lean | Fundamental properties of inner product spaces including Cauchy-Schwarz inequality, polarization identity, orthogonality tests, and norm equations |
| Adjoint.lean | Adjoint operators on Hilbert spaces; defines `ContinuousLinearMap.adjoint` satisfying `⟪x, A y⟫ = ⟪adjoint A x, y⟫`, and provides C⋆-algebra structure on `E →L[𝕜] E` |
| Orthogonal.lean | Orthogonal complements of submodules; defines `Kᗮ` notation for orthogonal complement and `U ⟂ V` for orthogonality of submodules |
| PiL2.lean | L² inner product structure on finite products of inner product spaces; defines `EuclideanSpace 𝕜 ι` and `OrthonormalBasis` as isometric equivalences to Euclidean space |
| Projection.lean | Import file aggregating projection theory (orthogonal projections onto closed subspaces); delegates to Projection subdirectory |
| GramSchmidtOrtho.lean | Gram-Schmidt orthogonalization and orthonormalization process; produces orthogonal/orthonormal systems from linearly independent vectors while preserving span |
| Spectrum.lean | Spectral theory for self-adjoint operators; proves eigenvalues are real, eigenspaces are orthogonal, and provides diagonalization theorem in finite dimensions |
| Rayleigh.lean | Rayleigh quotient `⟪T x, x⟫ / ‖x‖²` for self-adjoint operators; proves that extrema of the Rayleigh quotient correspond to eigenvectors and eigenvalues |
| l2Space.lean | Hilbert sum of families of inner product spaces; defines `lp G 2` with inner product structure, `IsHilbertSum` predicate, and `HilbertBasis` (isomorphism with `ℓ²(ι, 𝕜)`) |
| LaxMilgram.lean | Lax-Milgram theorem for coercive bilinear forms on Hilbert spaces; upgrades `continuousLinearMapOfBilin` to continuous equivalence for coercive forms |
| Subspace.lean | Theory of closed subspaces in inner product spaces and their orthogonal complements |
| Dual.lean | Riesz representation theorem for the dual space of Hilbert spaces; establishes isometric isomorphism between Hilbert space and its dual |
| Calculus.lean | Calculus in inner product spaces; differentiability of inner product and norm functions |
| LinearMap.lean | Linear maps between inner product spaces and their properties with respect to inner products |
| LinearPMap.lean | Partially defined linear maps on inner product spaces (for unbounded operators) |
| Orthonormal.lean | Orthonormal families and bases; defines orthonormality `⟪v i, v j⟫ = if i = j then 1 else 0` and proves properties of orthonormal sets |
| Positive.lean | Positive operators on inner product spaces; operators `T` satisfying `⟪T x, x⟫ ≥ 0` for all `x` |
| Symmetric.lean | Symmetric (self-adjoint) operators; operators satisfying `⟪T x, y⟫ = ⟪x, T y⟫` for all `x`, `y` |
| TensorProduct.lean | Inner product structure on tensor products of inner product spaces |
| TwoDim.lean | Two-dimensional inner product spaces; specific results for 2D geometry including area calculations and rotation properties |
| Laplacian.lean | Laplacian operator in inner product spaces; defines `Δf` and proves properties |
| GramMatrix.lean | Gram matrix of a family of vectors; matrix with entries `⟪v i, v j⟫` |
| JointEigenspace.lean | Joint eigenspaces for families of commuting operators |
| MeanErgodic.lean | Mean ergodic theorem in Hilbert spaces |
| Semisimple.lean | Semisimple operators (operators whose generalized eigenspaces are eigenspaces) |
| StarOrder.lean | Star order on positive operators in inner product spaces |
| Trace.lean | Trace of operators on finite-dimensional inner product spaces |
| WeakOperatorTopology.lean | Weak operator topology on bounded operators between Hilbert spaces |
| OfNorm.lean | Construction of inner product spaces from norm satisfying parallelogram law |
| NormPow.lean | Norm power inequalities in inner product spaces |
| EuclideanDist.lean | Euclidean distance in inner product spaces derived from the norm |
| Completion.lean | Completion of inner product spaces to Hilbert spaces |
| Continuous.lean | Continuity properties of inner product function |
| Convex.lean | Convexity results specific to inner product spaces |
| Affine.lean | Inner product structure on affine spaces |
| CanonicalTensor.lean | Canonical tensor product structure for inner product spaces |
| ConformalLinearMap.lean | Conformal linear maps (angle-preserving maps) in inner product spaces |
| MulOpposite.lean | Inner product structure on the opposite multiplication algebra |
| ProdL2.lean | L² inner product structure on binary products of inner product spaces |
| Orientation.lean | Orientations in inner product spaces using volume forms |

## Subdirectories

- [x] `Harmonic/` - Harmonic functions on real finite-dimensional inner product spaces; defines `HarmonicAt` and `HarmonicOnNhd` predicates for functions with vanishing Laplacian, proves that complex-analytic functions are harmonic (including real/imaginary parts, conjugates, and logarithms of norms)
- [x] `Projection/` - Orthogonal projection theory; proves Hilbert projection theorem (existence/uniqueness of minimizers), constructs projection operators `K.orthogonalProjection` and `K.starProjection`, develops reflection isometries, proves `K ⊔ Kᗮ = ⊤` and `Kᗮᗮ = K` for complete subspaces, and includes finite-dimensional results (dimension formula, Cartan-Dieudonné theorem on reflection factorization, orthogonal family decompositions)

## Search Tags

inner-product-space hilbert-space orthogonality projection adjoint-operator self-adjoint spectral-theory eigenvalues eigenvectors orthonormal-basis gram-schmidt cauchy-schwarz polarization-identity riesz-representation lax-milgram rayleigh-quotient l2-space hilbert-sum euclidean-space orthogonal-complement hilbert-basis diagonalization positive-operator symmetric-operator tensor-product laplacian gram-matrix mean-ergodic weak-operator-topology parallelogram-law completion functional-analysis
