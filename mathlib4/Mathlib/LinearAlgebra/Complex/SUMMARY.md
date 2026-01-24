---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Complex
generated: 2026-01-25T22:50:13Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Complex

## Overview

The `Complex/` subdirectory contains linear algebra theory specific to the complex numbers ℂ viewed as a vector space over the reals ℝ. Core content includes the ℝ-module structure on ℂ (with the standard basis {1, I} and corresponding basisOneI), finite-dimensionality results ([ℂ : ℝ] = 2), bundled linear maps for real/imaginary parts and conjugation, and a universal property (Complex.lift) for constructing algebra homomorphisms. The directory also provides decompositions of elements in complex star modules into real and imaginary parts (realPart and imaginaryPart), determinants of complex conjugation, and the standard orientation on ℂ as a 2-dimensional real vector space.

## Key Files

| File | Purpose |
|------|---------|
| Module.lean | Complex numbers as ℝ-vector space: SMul/module/algebra instances lifting ℝ-actions to ℂ-actions, basisOneI (standard basis {1, I}), bundled linear maps (reLm, imLm for real/imaginary parts), algebra morphisms (ofRealAm, conjAe for conjugation), universal property (Complex.lift constructing ℂ →ₐ[ℝ] A from square roots of -1), equivRealProdLm (ℂ ≃ₗ[ℝ] ℝ × ℝ), and decomposition of star module elements into realPart and imaginaryPart |
| FiniteDimensional.lean | Finite-dimensionality of ℂ over ℝ: FiniteDimensional ℝ ℂ instance (via basisOneI), dimension theorems (finrank ℝ ℂ = 2, rank ℝ ℂ = 2), dimension formulas for complex vector spaces over ℝ (finrank ℝ E = 2 * finrank ℂ E), and rational field results (rank ℚ ℝ = continuum, rank ℚ ℂ = continuum, ℂ ≃ₗ[ℚ] ℝ) |
| Determinant.lean | Determinants in complex vector space: det_conjAe (determinant of conjugation as linear map equals -1), linearEquiv_det_conjAe (determinant as linear equiv equals -1 in units) |
| Orientation.lean | Standard orientation on ℂ: Complex.orientation defined as basisOneI.orientation for the 2-dimensional real vector space structure |

## Subdirectories

*(No subdirectories)*

## Search Tags

complex-numbers vector-spaces real-vector-space module finite-dimensional basis conjugation real-part imaginary-part star-module determinant orientation algebra-homomorphism universal-property scalar-tower restrict-scalars linear-maps dimension-theory
