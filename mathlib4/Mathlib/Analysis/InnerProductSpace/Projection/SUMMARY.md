---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/InnerProductSpace/Projection
generated: 2025-12-05T08:15:32Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# Projection

## Overview

This directory contains the formalization of orthogonal projection theory for inner product spaces. It proves the existence of orthogonal projections (Hilbert projection theorem), constructs the orthogonal projection operators `K.orthogonalProjection : E →L[𝕜] K` and `K.starProjection : E →L[𝕜] E` for complete subspaces, and develops the theory of reflections in subspaces. The projection minimizes distance to the subspace and satisfies the fundamental orthogonality property `⟪u - K.starProjection u, w⟫ = 0` for all `w ∈ K`. Results include properties of orthogonal complements (double complement equals closure, sum with complement equals full space), projections in finite-dimensional spaces (Cartan–Dieudonné theorem on reflection generation), and decompositions via orthogonal families.

## Key Files

| File | Purpose |
|------|---------|
| Minimal.lean | Existence of minimizers (Hilbert projection theorem); proves that for any point `u` and nonempty complete convex set `K`, there exists unique `v ∈ K` minimizing `‖u - v‖`, with characterization via orthogonality condition |
| Basic.lean | Core projection definitions and API; constructs `K.orthogonalProjection : E →L[𝕜] K` (projection into subtype) and `K.starProjection : E →L[𝕜] E` (projection into ambient space), proves norm bounds `‖K.starProjection‖ ≤ 1`, orthogonality characterization, idempotence, self-adjointness, projection formula for singletons `(𝕜 ∙ v).starProjection w = (⟪v, w⟫ / ‖v‖²) • v`, and kernel equals orthogonal complement |
| Submodule.lean | Subspace-theoretic properties of projections; proves `K ⊔ Kᗮ = ⊤` and `Kᗮᗮ = K` for complete subspaces, double orthogonal complement equals topological closure `Kᗮᗮ = K.topologicalClosure`, complementarity `IsCompl K Kᗮ`, projection tendsto results for monotone families, and density criterion `Kᗮ = ⊥ ↔ K.topologicalClosure = ⊤` |
| Reflection.lean | Reflection isometries `K.reflection : E ≃ₗᵢ[𝕜] E` defined by `K.reflection u = 2 • K.starProjection u - u`; proves involutivity `K.reflection ∘ K.reflection = id`, characterization `K.reflection x = x ↔ x ∈ K`, reflection maps orthogonal complement elements to their negations, and specific formula for reflection across hyperplanes |
| FiniteDimensional.lean | Finite-dimensional projection theory; proves dimension formula `finrank K + finrank Kᗮ = finrank E`, determinant of reflection `det K.reflection = (-1)^(finrank Kᗮ)`, Cartan–Dieudonné theorem (every orthogonal isometry is product of at most `finrank E` reflections), orthogonal family decompositions `OrthogonalFamily.decomposition` for direct sum structure, and maximal orthonormal set characterization `(span 𝕜 v)ᗮ = ⊥ ↔ v is basis` |

## Subdirectories

No subdirectories.

## Search Tags

orthogonal-projection hilbert-projection-theorem minimizer complete-subspace star-projection orthogonality kernel-projection idempotent-projection self-adjoint-projection norm-projection lipschitz-projection reflection linear-isometry-equiv involution double-orthogonal-complement complementarity finite-dimensional cartan-dieudonne determinant-reflection orthogonal-family direct-sum decomposition orthonormal-basis dimension-formula projection-formula singleton-projection pythagorean-theorem dense-subspace
