---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Complex/UpperHalfPlane
generated: 2025-12-05T08:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# UpperHalfPlane

## Overview

The `UpperHalfPlane/` directory contains the formalization of the complex upper half-plane ℍ = {z ∈ ℂ : Im(z) > 0}, a fundamental object in complex analysis and modular form theory. It establishes ℍ as a subtype of ℂ, equips it with topological and metric structures (hyperbolic/Poincaré metric), defines the action of GL(2,ℝ) and SL(2,ℤ) by Möbius transformations, provides manifold structure, and studies functions bounded at infinity (relevant for modular forms).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines ℍ as {z : ℂ \| 0 < z.im}; basic structure including coercion to ℂ, real/imaginary parts, extensionality lemmas, additive action by ℝ, scalar action by positive reals, and positivity tactic extensions |
| Exp.lean | Exponential function properties on ℍ; proves norm bounds for q-expansions (qParam), showing ‖exp(2πiτ)‖ < 1 for τ ∈ ℍ (essential for modular form Fourier series convergence) |
| FunctionsBoundedAtInfty.lean | Defines filter `atImInfty` (approaching i∞), predicates `IsBoundedAtImInfty` and `IsZeroAtImInfty` for functions ℍ → α, submodules/subalgebras of bounded/vanishing functions (relevant for spaces of modular forms), tendsto lemmas for coercions |
| Manifold.lean | Complex manifold structure on ℍ; proves ℍ is a smooth manifold modeled on ℂ, coercion ℍ → ℂ is smooth, GL(2,ℝ)⁺ acts by smooth maps (Möbius transformations), includes smoothness of numerator/denominator/powers for automorphisms |
| Metric.lean | Hyperbolic (Poincaré) metric on ℍ given by dist(z,w) = 2·arsinh(dist(z,w as ℂ)/(2√(z.im·w.im))); proves triangle inequality, metric space instance, proper space, relates hyperbolic distance to Euclidean balls, proves SL(2,ℝ) acts by isometries |
| MoebiusAction.lean | GL(2,ℝ) action on ℍ by fractional linear transformations g·z = σ(g)((az+b)/(cz+d)) where σ is identity for positive determinant and conjugation otherwise; includes SL(2,ℤ) modular group action, special elements S (z ↦ -1/z) and T (z ↦ z+1), cocycle identities for denominators |
| Topology.lean | Topological space structure on ℍ (subspace topology from ℂ); proves ℍ is open embedding in ℂ, second-countable, T3/T4, contractible, locally path-connected, noncompact, locally compact; continuous GL(2,ℝ) action; vertical strips and modular group orbit lemmas; section ofComplex: ℂ → ℍ |

## Subdirectories

*(none)*

## Search Tags

upper-half-plane complex-analysis poincare-metric hyperbolic-geometry moebius-transformation modular-group fractional-linear-transformation GL2R SL2Z action manifold-structure bounded-at-infinity modular-forms q-expansion vertical-strip contractible-space isometry smooth-manifold
