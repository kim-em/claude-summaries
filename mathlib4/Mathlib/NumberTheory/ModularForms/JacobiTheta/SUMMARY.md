---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/ModularForms/JacobiTheta
generated: 2026-01-25T22:35:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# JacobiTheta

## Overview

The `JacobiTheta/` directory provides a comprehensive formalization of Jacobi theta functions in both one and two variables. It develops the two-variable theta function θ(z, τ) = ∑ exp(2πinz + πin²τ), proves its holomorphy (jointly in both variables) and functional equations via Poisson summation, then specializes to the one-variable case θ(τ) = ∑ exp(πin²τ) and establishes modular transformation properties. The implementation includes explicit bounds and convergence theorems, asymptotic decay estimates for applications to Hurwitz zeta and Dirichlet L-functions, and manifold differentiability formulations for the upper half-plane setting.

## Key Files

| File | Purpose |
|------|---------|
| TwoVariable.lean | Two-variable Jacobi theta function θ(z, τ) with holomorphy, functional equations relating (z, τ) to (z/τ, -1/τ), and derivative θ'(z, τ) for odd Dirichlet characters |
| OneVariable.lean | One-variable theta function θ(τ) as specialization θ₂(0, τ), with modular transformations θ(τ+2) = θ(τ) and θ(-1/τ) = √(-iτ)θ(τ), exponential decay bounds, and differentiability on ℍ |
| Bounds.lean | Asymptotic bounds for sums F_nat and F_int involving powers times exponentials, establishing O(exp(-pt)) decay for Hurwitz zeta and Dirichlet L-function applications |
| Manifold.lean | Manifold differentiability of jacobiTheta on the upper half-plane ℍ as a complex manifold, bridging differentiability and smooth manifold structure |

## Subdirectories

## Search Tags

jacobi-theta theta-functions modular-forms upper-half-plane poisson-summation functional-equations holomorphy two-variable one-variable exponential-decay asymptotic-bounds hurwitz-zeta dirichlet-L manifold-differentiability modular-transformations SL2Z
