---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/EulerProduct
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# EulerProduct

## Overview

The `EulerProduct/` directory establishes Euler product formulas for multiplicative functions, which express infinite sums as infinite products over primes. The main theoretical results prove that for multiplicative functions `f : ℕ → R` (on coprime arguments) in complete normed rings, `∏' p : Primes, ∑' e, f (p^e) = ∑' n, f n`, with specialized versions for completely multiplicative functions showing `∏' p : Primes, (1 - f p)⁻¹ = ∑' n, f n`. These abstract results are applied to prove the classical Euler products for the Riemann zeta function and Dirichlet L-series, valid for `Re(s) > 1`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core Euler product theorems: convergence of `∏' p : Primes, ∑' e, f (p^e)` to `∑' n, f n` for multiplicative functions on complete normed rings, with variants for completely multiplicative functions |
| DirichletLSeries.lean | Euler products for Riemann zeta and Dirichlet L-series: `∏' p : Primes, (1 - p^(-s))⁻¹ = ζ(s)` and `∏' p : Primes, (1 - χ p * p^(-s))⁻¹ = L(χ,s)` for `Re(s) > 1`, plus level-changing formulas |
| ExpLog.lean | Logarithmic form of Euler products: `exp(∑' p : Primes, -log(1 - f p)) = ∑' n, f n` for completely multiplicative `f : ℕ →*₀ ℂ` |

## Subdirectories

*(none)*

## Search Tags

euler-product multiplicative-function riemann-zeta dirichlet-L-series analytic-number-theory infinite-products primes completely-multiplicative summability smooth-numbers factored-numbers hasSum tprod convergence
