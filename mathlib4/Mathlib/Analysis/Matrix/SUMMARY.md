---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Matrix
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# Matrix

## Overview

The `Analysis/Matrix/` directory contains analytical results about matrices, focusing on Hermitian matrices, matrix norms, spectral theory, and positive (semi)definite matrices. This includes the spectral theorem for Hermitian matrices, LDL decomposition, continuous functional calculus for Hermitian matrices, various matrix norm definitions (elementwise, Frobenius, L∞ operator norm), and the relationship between positive definiteness and spectrum. The directory bridges linear algebra with analysis by providing normed spaces and inner product structures induced by matrices.

## Key Files

| File | Purpose |
|------|---------|
| Hermitian.lean | Proves that Hermitian matrices over ℝ and ℂ correspond to self-adjoint linear maps; shows diagonal elements of Hermitian matrices are real |
| HermitianFunctionalCalculus.lean | Implements continuous functional calculus for Hermitian matrices; realizes functional calculus as triple product `U * diagonal(f ∘ eigenvalues) * Uᴴ` using spectral theorem |
| LDL.lean | LDL decomposition of positive definite matrices: any positive definite matrix `S` can be decomposed as `S = LDLᴴ` where `L` is lower-triangular and `D` is diagonal |
| Normed.lean | Defines multiple matrix norm structures (not as instances since multiple choices exist): elementwise supremum norm, Frobenius norm `‖A‖ = sqrt(Σᵢⱼ ‖Aᵢⱼ‖²)`, and L∞ operator norm `‖A‖∞ = sup_i (Σⱼ ‖Aᵢⱼ‖)` |
| Order.lean | Constructs partial order on matrices via `A ≤ B ↔ (B - A).PosSemidef`; proves matrix algebra is a star-ordered ring; shows positive semidefinite matrices satisfy `xᴴAx = 0 ↔ Ax = 0` |
| PosDef.lean | Spectrum of positive (semi)definite matrices; proves eigenvalues of positive semidefinite matrices are nonnegative, eigenvalues of positive definite matrices are positive; constructs inner product spaces from positive semidefinite matrices via `⟪x, y⟫ = xᴴMy` |
| Spectrum.lean | Spectral theorem for Hermitian matrices (diagonalization via unitary change of basis); defines eigenvalues, eigenvector basis, and eigenvector unitary; proves `A = U * diag(eigenvalues) * Uᴴ`; shows spectrum equals range of eigenvalues |

## Subdirectories

*(none)*

## Search Tags

matrix-analysis hermitian-matrices spectral-theorem eigenvalues eigenvectors matrix-norms frobenius-norm operator-norm positive-definite positive-semidefinite ldl-decomposition functional-calculus diagonalization unitary-matrices self-adjoint inner-product-space star-ordered-ring matrix-order spectrum-theory
