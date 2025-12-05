---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/Gamma
generated: 2025-12-05T06:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# Gamma

## Overview

The `Gamma/` directory provides a comprehensive formalization of the Gamma function and closely related special functions (Beta function) for both real and complex variables. It defines the Gamma function via Euler's integral, establishes the fundamental functional equation Γ(s+1) = s·Γ(s), proves non-vanishing properties, derives differentiability, and establishes classical identities including Euler's reflection formula and Legendre's duplication formula. The directory also includes the Bohr-Mollerup theorem (uniquely characterizing Gamma via log-convexity) and Deligne's archimedean Gamma factors used in the theory of L-functions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of Γ function via Euler's integral ∫ exp(-x) x^(s-1); convergence proofs; functional equation Γ(s+1) = s·Γ(s); evaluation at naturals Γ(n+1) = n!; both real and complex cases |
| Beta.lean | Beta function Β(u,v) = ∫ x^(u-1) (1-x)^(v-1); relation Γ(u)Γ(v) = Γ(u+v)Β(u,v); non-vanishing of Γ; Euler sequence limit formula; Euler reflection formula Γ(s)Γ(1-s) = π/sin(πs); Legendre duplication formula; differentiability of 1/Γ |
| BohrMollerup.lean | Convexity and log-convexity of Γ on positive reals (via Hölder inequality); Bohr-Mollerup theorem (unique characterization of Γ as log-convex function satisfying functional equation and Γ(1)=1); weak form of Euler limit formula for log Γ; Legendre doubling formula for real positive arguments |
| Deligne.lean | Deligne's archimedean Gamma factors Γ_ℝ(s) = π^(-s/2) Γ(s/2) and Γ_ℂ(s) = 2(2π)^(-s) Γ(s) used in Dedekind zeta functions; functional equations for these factors; non-vanishing and evaluation results |
| Deriv.lean | Complex differentiability of Γ at all s ∉ {-n : n ∈ ℕ}; derivative formula via Mellin transform of log(t)·exp(-t); real differentiability counterpart; uses connection to Mellin transform theory |

## Subdirectories

(No subdirectories)

## Search Tags

gamma-function beta-function euler-integral functional-equation factorial reflection-formula legendre-duplication bohr-mollerup log-convex mellin-transform differentiability complex-analysis special-functions l-functions deligne archimedean-factors euler-limit-formula non-vanishing
