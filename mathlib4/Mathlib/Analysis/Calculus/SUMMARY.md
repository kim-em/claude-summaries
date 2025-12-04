---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 21
subdirs_count: 13
---

# Calculus

## Overview

The `Calculus/` directory contains the formalization of differential and integral calculus in normed spaces. It covers fundamental theorems (mean value theorem, implicit function theorem, inverse function theorem, Taylor's theorem), derivative computations (Fréchet derivatives, directional derivatives, iterated derivatives), smoothness classes (continuously differentiable functions), and important classical results (Darboux's theorem, L'Hôpital's rule, Rademacher's theorem, Lagrange multipliers). The directory includes both theoretical foundations (formal multilinear series for power series, differential slope functions) and practical tools (parametric integrals, uniform limits of derivatives, smooth series).

## Key Files

| File | Purpose |
|------|---------|
| FormalMultilinearSeries.lean | Defines formal multilinear series (families of n-multilinear maps) as the foundation for modeling sequences of derivatives; used to define C^n functions and analytic functions |
| MeanValue.lean | Proves the mean value inequality and equality theorems; includes Lipschitz bounds from derivative bounds, fencing inequalities, and the fundamental result that functions with zero derivative on convex sets are constant |
| Implicit.lean | Proves the implicit function theorem in multiple versions: general version for functions with complemented kernel, version for surjective derivatives with complemented kernels, and simplified version for finite-dimensional codomains |
| ImplicitContDiff.lean | Extends implicit function theorem to C^n smooth implicit functions |
| Taylor.lean | Proves Taylor's theorem for real functions with remainder estimates (Lagrange, Cauchy, mean remainder forms); defines Taylor polynomials and coefficients using iterated derivatives |
| LHopital.lean | Proves L'Hôpital's rule for 0/0 indeterminate forms; includes both interval-based and filter-based versions for computing limits of quotients via derivatives |
| Rademacher.lean | Proves Rademacher's theorem: Lipschitz functions between finite-dimensional real vector spaces are differentiable almost everywhere (Lebesgue measure); uses Morrey's proof via line differentiability |
| Darboux.lean | Proves Darboux's theorem: derivatives take all intermediate values (intermediate value property for derivatives) |
| VectorField.lean | Defines vector fields V : E → E on vector spaces; includes pullback under differentiable maps and Lie bracket with Leibniz identity |
| ParametricIntegral.lean | Proves differentiability of parametric integrals ∫ F(x,a) dμ(a) with respect to parameter x using dominated convergence; derivative equals integral of derivative |
| ParametricIntervalIntegral.lean | Specialized version of parametric integral differentiation for interval integrals |
| SmoothSeries.lean | Proves that infinite series of C^n functions are C^n when derivatives satisfy uniform summable bounds; includes differentiability and smoothness of function series |
| UniformLimitsDeriv.lean | Proves derivative of uniform limit equals limit of derivatives (swapping limits and derivatives via uniform convergence); includes the ε/3 proof technique |
| Monotone.lean | Proves monotone functions ℝ → ℝ are differentiable almost everywhere using Stieltjes measure and Radon-Nikodym derivatives |
| DSlope.lean | Defines differential slope dslope(f,a,b) = (f(b)-f(a))/(b-a) for b≠a and deriv(f,a) for b=a; proves continuity and differentiability properties |
| DerivativeTest.lean | Proves first and second derivative tests from calculus: local extrema characterized by sign changes in first derivative or sign of second derivative |
| LagrangeMultipliers.lean | Proves Lagrange multipliers method for conditional extrema: if φ has local extremum on f⁻¹({f(x₀)}), then differentials are linearly dependent |
| DiffContOnCl.lean | Studies functions differentiable on open sets with continuous extension to the closure |
| TangentCone.lean | Import file for tangent cone subdirectory (tangent cone concepts for optimization) |
| LogDeriv.lean | Logarithmic derivative (derivative of log ∘ f) |
| LogDerivUniformlyOn.lean | Uniform bounds on logarithmic derivatives |

## Subdirectories

- [x] `AddTorsor/` - Calculus on affine spaces and torsors (complete)
- [x] `BumpFunction/` - Smooth bump functions (smooth functions with compact support) (complete)
- [x] `Conformal/` - Conformal maps (angle-preserving differentiable maps) (complete)
- [ ] `ContDiff/` - Continuously differentiable functions (C^n smoothness classes) (pending)
- [ ] `Deriv/` - One-dimensional derivatives (real and complex derivatives) (pending)
- [ ] `DifferentialForm/` - Differential forms on normed spaces (pending)
- [ ] `FDeriv/` - Fréchet derivatives (multivariable derivatives in normed spaces) (pending)
- [ ] `Gradient/` - Gradient of functions (vector of partial derivatives in inner product spaces) (pending)
- [ ] `InverseFunctionTheorem/` - Inverse function theorem (local invertibility from invertible derivative) (pending)
- [ ] `IteratedDeriv/` - Iterated derivatives (nth derivatives) (pending)
- [ ] `LineDeriv/` - Directional derivatives (derivatives along lines/vectors) (pending)
- [ ] `LocalExtr/` - Local extrema and critical points (Fermat's theorem) (pending)
- [ ] `TangentCone/` - Tangent cones and normal cones for convex analysis and optimization (pending)

## Search Tags

calculus differential-calculus derivatives fréchet-derivative directional-derivative iterated-derivative mean-value-theorem implicit-function-theorem inverse-function-theorem taylor-theorem lhopital darboux rademacher lagrange-multipliers parametric-integrals smooth-series uniform-convergence monotone-differentiability derivative-tests vector-fields lie-bracket formal-multilinear-series bump-functions conformal-maps continuously-differentiable local-extrema tangent-cone gradient slope
