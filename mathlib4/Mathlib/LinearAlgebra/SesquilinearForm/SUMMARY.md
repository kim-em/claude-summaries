---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/SesquilinearForm
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# SesquilinearForm

## Overview

The `SesquilinearForm/` directory provides the theory of sesquilinear maps and forms, generalizing bilinear maps to allow different ring homomorphisms on each argument. Sesquilinear maps have the form `M₁ →ₛₗ[I₁] M₂ →ₛₗ[I₂] M` where `I₁` and `I₂` are ring homomorphisms. The directory covers orthogonality relations, symmetry and alternating properties, positive semidefiniteness, orthogonal complements, adjoint pairs, and nondegeneracy conditions. Special cases include bilinear forms (when both homomorphisms are identity) and Hermitian forms (with conjugate-linear structure). Star.lean extends this theory to sesquilinear forms over star rings, connecting to matrix representations and Hermitian/positive definite properties.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core sesquilinear form theory: orthogonality (IsOrtho, IsOrthoᵢ with linear independence), reflexivity (IsRefl with kernel properties), symmetry (IsSymm), positive semidefiniteness (IsNonneg, IsPosSemidef), alternating forms (IsAlt), orthogonal complements (Submodule.orthogonalBilin), adjoint pairs (IsAdjointPair, IsPairSelfAdjoint), and nondegeneracy (separatingLeft/Right, Nondegenerate with kernel characterizations) |
| Star.lean | Sesquilinear forms over star rings: symmetry characterization via basis (isSymm_iff_basis, isSymm_iff_isHermitian_toMatrix connecting to matrix Hermitian property), matrix representation (star_dotProduct_toMatrix₂_mulVec, apply_eq_star_dotProduct_toMatrix₂_mulVec), and positive semidefiniteness (isPosSemidef_iff_posSemidef_toMatrix linking form and matrix properties) |

## Subdirectories

(none)

## Search Tags

sesquilinear-forms bilinear-forms hermitian-forms orthogonality symmetry alternating positive-semidefinite orthogonal-complement adjoint-pairs nondegeneracy star-rings matrix-representation linear-algebra semilinear-maps
