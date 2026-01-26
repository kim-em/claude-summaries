---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Moments
generated: 2026-01-26T20:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 10
subdirs_count: 0
---

# Moments

## Overview

The `Moments/` directory contains formalization of moment-related theory for probability measures, centered around the moment-generating function (MGF) and cumulant-generating function (CGF). It defines moments, central moments, variance, covariance, and their analytical properties, as well as sub-Gaussian random variables and the Chernoff/Hoeffding concentration inequalities. This includes extensive theory on the MGF as an analytic function, integrability conditions for exponential functions of random variables, and characterization results showing that MGFs determine distributions uniquely.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: moment `μ[X^p]`, central moment `μ[(X-𝔼[X])^p]`, moment-generating function `mgf X μ t = μ[exp(t*X)]`, cumulant-generating function `cgf = log ∘ mgf`. Proves independence properties (mgf and cgf are additive for independent variables), Chernoff bounds on tail probabilities. |
| Variance.lean | Variance theory: defines `evariance` (ℝ≥0∞-valued) and `variance` (ℝ-valued) with notation `eVar[X;μ]` and `Var[X;μ]`. Proves Chebyshev's inequality, variance formulas (`Var[X] = 𝔼[X²] - 𝔼[X]²`), addition/scaling properties, Bhatia-Davis and Popoviciu's inequalities for bounded random variables. |
| Covariance.lean | Covariance definition `cov[X,Y;μ] = ∫ω, (X ω - μ[X])*(Y ω - μ[Y]) ∂μ` with linearity, scaling, and independence properties. Proves covariance vanishes for independent random variables. |
| CovarianceBilinDual.lean | Covariance as continuous bilinear forms on dual spaces for Banach space-valued measures: `covarianceBilinDual μ : StrongDual ℝ E →L[ℝ] StrongDual ℝ E →L[ℝ] ℝ` with value `∫x, (L₁ x - μ[L₁])*(L₂ x - μ[L₂]) ∂μ`. Includes uncentered version and auxiliary `StrongDual.toLp` continuous linear map from dual to Lp spaces. |
| CovarianceBilin.lean | Covariance bilinear form for Hilbert space-valued measures: `covarianceBilin μ : E →L[ℝ] E →L[ℝ] ℝ` mapping `x,y` to `cov[⟪x,·⟫, ⟪y,·⟫; μ]`. Defines covariance operator `covarianceOperator μ : E →L[ℝ] E` satisfying `⟪covarianceOperator μ x, y⟫ = ∫z, ⟪x,z⟫*⟪y,z⟫ ∂μ`, proves positive semidefiniteness. |
| IntegrableExpMul.lean | Domain theory for MGF: defines `integrableExpSet X μ = {t | Integrable (exp(t*X)) μ}` and proves it's a convex interval containing 0. For `t` in the interior, proves integrability of `X^p * exp(v*X)` for all `p≥0`, implying finite moments and ℒp membership. Critical for establishing where MGF/CGF are well-defined. |
| ComplexMGF.lean | Complex extension `complexMGF X μ z = μ[cexp(z*X)]`, analytic on vertical strip `{z | z.re ∈ interior(integrableExpSet X μ)}`. Proves `complexMGF X μ (t*I) = charFun(μ.map X) t` (characteristic function on imaginary axis), derivatives formula `iteratedDeriv n (complexMGF X μ) z = μ[X^n * cexp(z*X)]`, and uniqueness result: equal complex MGFs imply equal distributions. |
| MGFAnalytic.lean | Analyticity of real MGF: proves `mgf X μ` is analytic on `interior(integrableExpSet X μ)` with derivatives `deriv (mgf X μ) t = μ[X*exp(t*X)]` and `iteratedDeriv n (mgf X μ) t = μ[X^n*exp(t*X)]`. Proves CGF is also analytic, with formulas for CGF derivatives including `iteratedDeriv 2 (cgf X μ) t = Var[X; μ.tilted(t*X·)]`. |
| Tilted.lean | Relates tilted measures to MGF/CGF: for `μ.tilted (t*X·)` (exponentially tilted measure), proves `(μ.tilted(t*X·))[X] = deriv(cgf X μ) t` and `Var[X; μ.tilted(t*X·)] = iteratedDeriv 2 (cgf X μ) t`. Key tool for connecting MGF derivatives to variance under tilted distributions. |
| SubGaussian.lean | Sub-Gaussian random variables: defines `HasSubgaussianMGF X c μ` (MGF bounded by `exp(c*t²/2)` for all `t`), conditionally sub-Gaussian `HasCondSubgaussianMGF`, and kernel-parameterized version. Proves Hoeffding's lemma (bounded centered random variables are sub-Gaussian), Hoeffding inequality for sums of independent sub-Gaussians, and Azuma-Hoeffding inequality for martingale differences. |

## Subdirectories

None - this is a leaf directory.

## Search Tags

moments variance covariance moment-generating-function mgf cgf cumulant analytic sub-gaussian hoeffding chernoff chebyshev tilted-measure characteristic-function complex-analysis integrability exponential-integrability banach-space hilbert-space bilinear-form concentration-inequality martingale

