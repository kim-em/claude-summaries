---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/BumpFunction
generated: 2025-12-04T09:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# BumpFunction

## Overview

The `BumpFunction/` directory formalizes smooth bump functions—infinitely smooth (C^∞) functions with compact support that are equal to 1 on an inner ball and smoothly decay to 0 on an outer ball. These functions are fundamental tools in real analysis, used to construct partitions of unity and approximate continuous functions by smooth ones. The directory establishes bump function existence for two classes of spaces (inner product spaces and finite-dimensional spaces), provides normalized versions for convolution, proves density of smooth functions in continuous functions, and demonstrates convergence of convolutions to identity.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines core bump function structures: `ContDiffBump c` (bundled smooth bump centered at c with radii rIn < rOut), `ContDiffBumpBase E` (parametric family of bump functions), and typeclass `HasContDiffBump E` registering that E admits bump functions; establishes properties: f = 1 on closedBall(c, rIn), support(f) = ball(c, rOut), 0 ≤ f ≤ 1, and C^∞ smoothness in all parameters |
| InnerProduct.lean | Constructs bump functions for inner product spaces using `ContDiffBumpBase.ofInnerProductSpace`; uses smoothTransition((R - ‖x‖)/(R - 1)) which exploits norm smoothness away from zero; provides instance `hasContDiffBump_of_innerProductSpace` |
| FiniteDimension.lean | Constructs bump functions for finite-dimensional spaces via convolution: proves any open set has smooth support (`IsOpen.exists_smooth_support_eq`), builds auxiliary function u with support = ball(0,1), defines w_D (scaled/normalized u), and constructs y_D = w_D ⋆ indicator(closedBall(0,1)) giving smooth function equal to 1 on ball(0, 1-D) with support ball(0, 1+D); provides instance for `HasContDiffBump` on finite-dimensional spaces |
| Normed.lean | Defines normalized bump functions `f.normed μ x = f x / ∫ f dμ` with integral 1; proves properties: integral_normed = 1, nonneg_normed, support_normed_eq = ball(c, rOut), bounds relating normalized values to measure of inner/outer balls (for Haar measures), and tendsto_support_normed_smallSets for shrinking supports |
| Convolution.lean | Proves convolution identities and approximation theorems: `convolution_eq_right` (φ ⋆ g = (∫ φ) • g when g constant on support), `normed_convolution_eq_right` (normalized version gives identity), `dist_normed_convolution_le` (distance estimate when g near constant), `convolution_tendsto_right` (φ_i ⋆ g_i → g as rOut → 0), and `ae_convolution_tendsto_right_of_locallyIntegrable` (a.e. convergence to identity for locally integrable functions via Lebesgue differentiation) |
| SmoothApprox.lean | Proves density of smooth functions in continuous functions: `ContinuousMap.dense_setOf_contDiff` shows C^∞ functions are dense in C(E,F) for finite-dimensional E and Banach F; includes `exists_contDiff_dist_le` for uniform approximation via convolution with bump functions; wraps measure-theoretic convolution results into user-friendly approximation theorems |

## Subdirectories

*(none)*

## Search Tags

bump-functions smooth-functions compact-support partitions-of-unity convolution approximation-theory inner-product-spaces finite-dimensional-spaces smooth-approximation density-theorems normalized-bump-functions lebesgue-differentiation smooth-transition contdiff haar-measure
