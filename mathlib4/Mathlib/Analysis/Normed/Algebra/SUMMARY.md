---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Algebra
generated: 2025-12-05T08:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 12
subdirs_count: 0
---

# Algebra

## Overview

The `Algebra/` directory contains theory and results specific to normed algebras (Banach algebras), focusing on spectrum theory, exponential maps, and structural theorems. This includes the fundamental results of Gelfand-Mazur theorem (showing complex Banach division algebras are isomorphic to ℂ), Gelfand's formula for spectral radius, and comprehensive treatments of the exponential function in various algebraic structures (matrices, quaternions, dual numbers, trivial square zero extensions). The directory also covers unitization of non-unital algebras with appropriate norm structures, ultrametric preservation in normed algebras, and character space compactness.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Character space compactness via Banach-Alaoglu theorem; shows `characterSpace 𝕜 A` is compact for normed algebras over proper spaces; bounds character norms by `‖1‖` |
| Spectrum.lean | Core spectrum theory for Banach algebras; defines spectral radius; proves spectrum is closed, compact, and contained in closed ball of norm radius; shows resolvent set is open; includes resolvent differentiability |
| Exponential.lean | Exponential map `NormedSpace.exp 𝕂 : 𝔸 → 𝔸` in topological algebras; proves `exp(x+y) = exp(x) * exp(y)` for commuting elements; shows infinite radius of convergence for ℝ and ℂ; includes `exp(-x) = exp(x)⁻¹` for division rings |
| GelfandFormula.lean | Gelfand's formula for spectral radius in complex Banach algebras: `spectralRadius ℂ a = limsup (‖aⁿ‖^(1/n))`; proves spectrum is nonempty in complex Banach algebras; includes resolvent differentiability |
| GelfandMazur.lean | Gelfand-Mazur theorem: nontrivial normed ℂ-algebras with multiplicative norm are isomorphic to ℂ; real case: normed ℝ-algebras are isomorphic to ℝ or ℂ; includes Ostrowski's variant and detailed proofs using polynomial factorization |
| Unitization.lean | Norm structures on `Unitization 𝕜 A` for non-unital algebras; defines `splitMul` map to `𝕜 × (A →L[𝕜] A)`; proves unitization is Banach algebra with `‖1‖ = 1` when A has regular norm; shows natural inclusion `A → Unitization 𝕜 A` is isometry |
| UnitizationL1.lean | Alternative L¹ norm on `WithLp 1 (Unitization 𝕜 A)` as type synonym; defines `‖(k,a)‖ = ‖k‖ + ‖a‖`; provides algebra isomorphism between unitization and its L¹ variant; used for quasispectrum compactness proofs |
| MatrixExponential.lean | Matrix exponential results: `exp_transpose`, `exp_conjTranspose`, `exp_diagonal`, `exp_blockDiagonal`; copies `NormedSpace.exp` lemmas to matrices hiding norm choice; proves `exp_add_of_commute` for matrices without fixing canonical norm |
| QuaternionExponential.lean | Quaternion exponential `exp ℝ : ℍ[ℝ] → ℍ[ℝ]`; general expansion via `Real.cos` and `Real.sin`; special case for pure imaginary quaternions; proves `‖exp q‖ = exp ‖re q‖` |
| TrivSqZeroExt.lean | Exponential for trivial square-zero extensions; defines L¹ norm `‖r + m‖ = ‖r‖ + ‖m‖`; proves `exp_inl`, `exp_inr`, `fst_exp`, `snd_exp`; provides complete normed algebra instance hierarchy |
| DualNumber.lean | Dual number exponential results; restatements of `TrivSqZeroExt` results; proves `exp eps = 1 + eps` and `exp (r • eps) = 1 + r • eps` |
| Ultra.lean | Ultrametricity preservation in normed algebras; proves normed division ring over ultrametric field is ultrametric; bidirectional: ultrametic normed algebra implies ultrametric base field (with `‖1‖ = 1`) |

## Subdirectories

(none)

## Search Tags

banach-algebras normed-algebras spectrum spectral-radius resolvent-set gelfand-formula gelfand-mazur exponential-map character-space unitization matrix-exponential quaternion-exponential dual-numbers trivial-square-zero-extensions ultrametric-algebras ostrowski-theorem complex-banach-algebras functional-calculus banach-alaoglu analytic-functions radius-of-convergence l1-norm regular-normed-algebra
