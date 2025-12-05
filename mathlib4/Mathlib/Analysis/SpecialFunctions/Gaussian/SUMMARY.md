---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/Gaussian
generated: 2025-12-05T06:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Gaussian

## Overview

The `Gaussian/` directory contains formalized theory of Gaussian functions and the Gaussian integral. It proves the classic formula ∫ exp(-bx²) = √(π/b) for real and complex parameters, extends this to finite-dimensional inner product spaces, computes the Fourier transform of Gaussians (showing the Fourier transform of a Gaussian is another Gaussian), and applies Poisson summation to derive Jacobi's theta-function transformation formula. These results connect measure theory, Fourier analysis, complex analysis, and special functions (including the evaluation Γ(1/2) = √π).

## Key Files

| File | Purpose |
|------|---------|
| GaussianIntegral.lean | Core Gaussian integral formula ∫ exp(-bx²) dx = √(π/b); includes integrability results for x^s exp(-bx²), proof using polar coordinates for the squared integral, continuity in the parameter b, extension to complex b with positive real part, half-line variants, and special value Γ(1/2) = √π |
| FourierTransform.lean | Fourier transform of Gaussian functions; proves ∫ exp(itx) exp(-bx²) dx = √(π/b) exp(-t²/4b) for complex b with Re(b) > 0; includes general quadratic exponential formula ∫ exp(bx² + cx + d) dx, extensions to finite-dimensional inner product spaces, and versions scaled with π factor for symmetric formulas |
| PoissonSummation.lean | Application of Poisson summation to Gaussians; proves Jacobi's theta transformation ∑ exp(-πan²) = (1/√a) ∑ exp(-πn²/a) for complex a with positive real part; includes rapid decay estimates for Gaussian-type functions along cocompact ℝ and general quadratic form version with linear term |

## Subdirectories

(none)

## Search Tags

gaussian-integral fourier-transform poisson-summation theta-function jacobi gaussian-function exp-neg-square polar-coordinates measure-theory complex-analysis gamma-function special-values inner-product-spaces finite-dimensional quadratic-exponential integrability asymptotics fourier-analysis
