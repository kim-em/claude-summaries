---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/Gradient
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Gradient

## Overview

The `Gradient/` directory formalizes the gradient of functions from Hilbert spaces to scalars (ℝ or ℂ). The gradient is defined as the unique vector `f'` in the domain space such that the function's linear approximation is given by the inner product `⟨f', x' - x⟩`. This connects the Fréchet derivative (a continuous linear map) to the Riesz representation theorem, converting dual space elements to vectors via the inner product structure. The file establishes translations between gradient concepts and existing Fréchet/ordinary derivative theory, proves uniqueness and differentiability results, and handles the one-dimensional case where gradients reduce to conjugated derivatives.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines gradient concepts (HasGradientAt, HasGradientWithinAt, gradient operator ∇) and establishes equivalences with Fréchet derivatives via the Riesz representation toDual isomorphism; proves uniqueness of gradients, translations to/from ordinary derivatives in dimension one, congruence lemmas, gradients of constant functions (zero), and continuity properties of functions admitting gradients |

## Subdirectories

*(No subdirectories)*

## Search Tags

gradient inner-product-space hilbert-space riesz-representation frechet-derivative deriv toDual differentiable continuity uniqueness one-dimensional congruence constant-function calculus analysis optimization
