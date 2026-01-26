---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Distributions/Gaussian
generated: 2026-01-26T21:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Gaussian

## Overview

The `Gaussian/` directory provides a comprehensive formalization of Gaussian (normal) distributions, starting with the real line and extending to arbitrary Banach and Hilbert spaces. It defines the `IsGaussian` predicate characterizing measures whose push-forwards under continuous linear forms are Gaussian, proves characterization via characteristic functions, establishes Fernique's theorem (exponential integrability of the squared norm), and derives fundamental properties including transformations, convolutions, products, and moment calculations. The theory covers both the one-dimensional case with explicit PDF/CDF formulas and the general infinite-dimensional case using characteristic function methods.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `IsGaussian` predicate for measures on Banach spaces (measure is Gaussian iff all continuous linear form push-forwards are real Gaussians), proves Gaussian measures are probability measures, establishes closure under continuous linear maps and equivalences, proves characterization theorem `isGaussian_iff_charFunDual_eq` relating Gaussianity to characteristic function form, and shows Gaussians are closed under convolution, translation, negation, and products |
| CharFun.lean | Proves Gaussian measures are uniquely determined by mean and covariance via characteristic functions, establishes `isGaussian_iff_gaussian_charFunDual` (Gaussian iff charFunDual has form `exp(L m * I - f L L / 2)` for some positive semidefinite bilinear form), proves uniqueness theorem `gaussian_charFunDual_congr` showing `m` and `f` must equal the mean and covariance bilinear form, includes Hilbert space specialization with inner product formulation |
| Fernique.lean | Proves rotation invariance of centered Gaussian products and Fernique's theorem `exists_integrable_exp_sq` (for Gaussian measures there exists C>0 such that exp(C*‖x‖²) is integrable), derives finite moments of all orders `memLp_id`, proves Gaussian measures are either Dirac or have no atoms, establishes centered Gaussian product invariance under rotation by arbitrary angle θ |
| Real.lean | Real Gaussian distribution `gaussianReal μ v` with mean μ and variance v, defines PDF `gaussianPDFReal μ v x = (√(2πv))⁻¹ * exp(-(x-μ)²/(2v))`, proves PDF integrates to 1, establishes transformation laws (translation, scaling, negation), computes characteristic function `charFun t = exp(t*μ*I - v*t²/2)`, MGF, and CGF, proves moments (mean=μ, variance=v, all finite moments), shows convolution `gaussianReal m₁ v₁ ∗ gaussianReal m₂ v₂ = gaussianReal (m₁+m₂) (v₁+v₂)`, and proves uniqueness via `gaussianReal_ext_iff` |

## Subdirectories

None

## Search Tags

gaussian-distribution normal-distribution probability-theory measure-theory banach-space hilbert-space characteristic-function moment-generating-function fernique-theorem rotation-invariance pdf probability-density-function isGaussian convolution transformation covariance mean variance exponential-integrability finite-moments continuous-linear-map inner-product-space charFun charFunDual mgf cgf gaussianReal gaussianPDF second-countable borel-space
