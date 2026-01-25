---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/Harmonic
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# Harmonic

## Overview

The `Harmonic/` directory formalizes the theory of harmonic numbers (the sequence H_n = 1 + 1/2 + 1/3 + ... + 1/n), with deep connections to the Euler-Mascheroni constant γ and the Riemann zeta function. It includes proofs that harmonic numbers are never integers (using p-adic valuations), logarithmic bounds, the convergence of H_n - log(n) to γ, derivatives of the Gamma function at positive integers, and asymptotics of the Riemann zeta function near s = 1. The module bridges classical number theory, analysis, and special functions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of harmonic numbers as `harmonic n = ∑ i in range n, (i + 1)⁻¹`, with basic recursion lemmas |
| Bounds.lean | Logarithmic bounds proving `log(n + 1) ≤ H_n ≤ 1 + log(n)` using integral comparison |
| Int.lean | Proof that H_n is not an integer for n ≥ 2, using Kürschák's argument via 2-adic valuations |
| EulerMascheroni.lean | Definition of Euler-Mascheroni constant γ as limit of `H_n - log(n+1)`, with bounds `1/2 < γ < 2/3` |
| GammaDeriv.lean | Explicit formula for derivative of Gamma function at positive integers: `deriv Γ(n+1) = n! * (-γ + H_n)`, proven via Bohr-Mollerup convexity theorem |
| ZetaAsymp.lean | Asymptotics of Riemann zeta function: `ζ(s) - 1/(s-1) → γ` as `s → 1`, with evaluation of `ζ(1)` under Mathlib's conventions |

## Subdirectories

(none)

## Search Tags

harmonic-numbers euler-mascheroni-constant riemann-zeta gamma-function p-adic-valuation logarithmic-bounds analytic-number-theory bohr-mollerup special-functions dirichlet-series asymptotic-analysis hurwitz-zeta
