---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/LSeries
generated: 2026-01-25T23:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 20
subdirs_count: 0
---

# LSeries

## Overview

The `LSeries/` directory contains a comprehensive formalization of L-series theory in complex analysis and analytic number theory. This includes the general theory of L-series (Dirichlet series of the form `∑ f(n)/n^s`), their convergence properties, analytic continuation, and functional equations. Major special cases covered include the Riemann zeta function, Hurwitz zeta function, Dirichlet L-functions (for Dirichlet characters), and L-series of arithmetic functions like the Möbius and von Mangoldt functions. The directory culminates in a complete proof of Dirichlet's theorem on primes in arithmetic progressions, which relies critically on the non-vanishing of Dirichlet L-functions on the line `Re(s) = 1`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core L-series definitions: `LSeries f s = ∑' n, f(n)/n^s`, summability, convergence criteria, and abscissa of convergence |
| Convergence.lean | Abscissa of absolute convergence `LSeries.abscissaOfAbsConv` as an `EReal` value and convergence theorems |
| Linearity.lean | Linearity properties of L-series under addition and scalar multiplication |
| Convolution.lean | Dirichlet convolution of arithmetic functions and its effect on L-series |
| Deriv.lean | Derivatives of L-series with respect to the complex parameter `s` |
| SumCoeff.lean | Summation of L-series coefficients and related identities |
| MellinEqDirichlet.lean | Connection between Mellin transforms and Dirichlet series representations |
| Positivity.lean | Positivity properties of L-series with non-negative real coefficients |
| RiemannZeta.lean | Definition and properties of the Riemann zeta function `ζ(s)`, completed zeta `Λ(s) = π^(-s/2) Γ(s/2) ζ(s)`, functional equation `s ↔ 1-s` |
| HurwitzZeta.lean | Hurwitz zeta function `∑' n, 1/(n+a)^s` and exponential zeta function, meromorphic continuation, functional equations |
| HurwitzZetaEven.lean | Theory of even Hurwitz zeta functions (large file, 39KB, detailed functional equation proofs) |
| HurwitzZetaOdd.lean | Theory of odd Hurwitz zeta functions and their analytic properties |
| HurwitzZetaValues.lean | Special values of Hurwitz and Riemann zeta at integers in terms of Bernoulli numbers |
| ZMod.lean | L-series of functions on `ZMod N`, analytic continuation, completed L-functions with Gamma factors, functional equations |
| Dirichlet.lean | L-series of Dirichlet characters and arithmetic functions (Möbius, von Mangoldt), relation to logarithmic derivatives of zeta |
| DirichletContinuation.lean | Analytic continuation of Dirichlet L-functions, completed L-functions, global root numbers, functional equations for primitive characters |
| Nonvanishing.lean | Non-vanishing of Dirichlet L-functions on `Re(s) ≥ 1` (except trivial character at `s=1`), crucial for PNT and Dirichlet's theorem |
| AbstractFuncEq.lean | Abstract framework for functional equations via Mellin transforms, weak and strong FE-pairs arising from modular forms |
| Injectivity.lean | Injectivity properties of L-series (distinguishing characters from their L-functions) |
| PrimesInAP.lean | Complete proof of Dirichlet's theorem: infinitely many primes in arithmetic progressions `p ≡ a (mod q)` when `gcd(a,q)=1` |

## Subdirectories

*(No subdirectories)*

## Search Tags

L-series Dirichlet-series Riemann-zeta Hurwitz-zeta Dirichlet-L-functions analytic-continuation functional-equation meromorphic-continuation Dirichlet-characters arithmetic-functions von-Mangoldt Mobius abscissa-of-convergence Gamma-factors root-number Mellin-transform modular-forms primes-in-arithmetic-progressions Dirichlet-theorem non-vanishing prime-number-theory zeta-values Bernoulli-numbers complex-analysis number-theory
