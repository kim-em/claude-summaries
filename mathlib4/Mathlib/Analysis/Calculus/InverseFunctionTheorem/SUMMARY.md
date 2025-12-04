---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/InverseFunctionTheorem
generated: 2025-12-04T07:15:16Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# InverseFunctionTheorem

## Overview

This directory contains the complete formalization of the inverse function theorem in normed spaces, starting from the fundamental notion of approximation and building up to smooth (C^n) inverse functions. The approach centers on `ApproximatesLinearOn`, a predicate stating that `‖f x - f y - f' (x - y)‖ ≤ c * ‖x - y‖` on a set, which allows splitting the proof into small, reusable lemmas. The directory proves local invertibility from invertible derivatives, provides explicit inverse functions with derivatives, and extends results to continuously differentiable and one-dimensional cases.

## Key Files

| File | Purpose |
|------|---------|
| ApproximatesLinearOn.lean | Defines the core predicate `ApproximatesLinearOn f f' s c` stating `f` approximates linear map `f'` with constant `c` on set `s`; proves that such maps are locally onto (via Banach fixed-point-style iteration), construct `OpenPartialHomeomorph` from the approximation, and shows the inverse function also approximates the inverse linear map |
| FDeriv.lean | Main inverse function theorem for Fréchet derivatives: if `f` has strict derivative `f'` (a linear equiv) at `a`, constructs `toOpenPartialHomeomorph` and proves the inverse function `localInverse` has strict derivative `f'.symm` at `f a`; also proves functions with invertible strict derivatives everywhere are open maps |
| Deriv.lean | One-dimensional specialization of inverse function theorem for `f : 𝕜 → 𝕜` (normed field); translates `HasStrictDerivAt f f' a` with `f' ≠ 0` into the Fréchet version using `ContinuousLinearEquiv.unitsEquivAut`, constructs local inverse with derivative `f'⁻¹`, and proves open mapping theorem for 1D case |
| ContDiff.lean | Extends inverse function theorem to C^n-smooth functions: if `f` is `ContDiffAt 𝕂 n` at `a` (with `n ≥ 1`) and has invertible derivative `f'` at `a`, the local inverse is also `ContDiffAt 𝕂 n` at `f a`; uses `hasStrictFDerivAt'` to connect smoothness with strict differentiability |
| FiniteDimensional.lean | Proves that in finite-dimensional real spaces, a function approximating a linear equivalence on a subset can be extended to a global homeomorphism of the entire space; uses Lipschitz extension theorem with `lipschitzExtensionConstant` to extend `f - f'` from `s` to all of `E` |

## Subdirectories

None - this is a leaf directory.

## Search Tags

inverse-function-theorem local-invertibility strict-derivative frechet-derivative approximates-linear-on open-partial-homeomorph local-inverse continuously-differentiable smooth-inverse one-dimensional-inverse finite-dimensional-extension lipschitz-approximation banach-fixed-point nonlinear-right-inverse open-map homeomorphism-extension
