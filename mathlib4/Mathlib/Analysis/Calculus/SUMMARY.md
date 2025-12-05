---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus
generated: 2025-12-05T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 21
subdirs_count: 13
---

# Calculus

## Overview

The `Calculus/` directory contains the comprehensive formalization of differential and integral calculus in normed spaces, providing both the theoretical foundations and computational machinery for differentiation in Mathlib. The directory is organized around three main derivative notions: Fréchet derivatives (`FDeriv/`) for multivariable calculus in normed spaces, ordinary derivatives (`Deriv/`) for one-dimensional real and complex functions, and directional/line derivatives (`LineDeriv/`) for weaker differentiability along specific directions. Building on these foundations, the directory establishes smoothness classes (`ContDiff/`) using formal multilinear series to define C^n functions, iterated derivatives (`IteratedDeriv/`) with Faà di Bruno's formula for compositions, and specialized derivative structures (gradients in Hilbert spaces, differential forms, conformal maps).

The directory proves the fundamental theorems of calculus: mean value theorem with applications to monotonicity and Lipschitz bounds, implicit function theorem for C^n smooth implicit functions, inverse function theorem extending to smooth inverses, and Taylor's theorem with multiple remainder forms. Classical results include Darboux's theorem (intermediate value property for derivatives), L'Hôpital's rule for indeterminate forms, Rademacher's theorem (Lipschitz functions are almost everywhere differentiable), Rolle's theorem with applications to polynomial root counting, and Lagrange multipliers for constrained optimization. The directory also provides important technical infrastructure: tangent cones and unique differentiability (`TangentCone/`) to ensure derivative uniqueness, bump functions (`BumpFunction/`) for smooth approximation and partitions of unity, and tools for parametric integrals, uniform convergence of derivatives, and smooth function series.

Beyond the theoretical core, the directory includes practical computational tools: derivative formulas for all standard operations (composition via chain rule, products, quotients, powers), specialized results for affine spaces and torsors (`AddTorsor/`), vector fields with Lie brackets, conformal geometry (`Conformal/`), differential forms with exterior derivatives (`DifferentialForm/`), local extrema theory (`LocalExtr/`) with Fermat's theorem, and analysis of functions differentiable on open sets with continuous extensions to the closure. This makes the directory both a complete reference for theoretical calculus and a practical toolkit for differentiation in formalized mathematics.

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
- [x] `ContDiff/` - Continuously differentiable functions (C^n smoothness classes) (complete)
- [x] `Deriv/` - One-dimensional derivatives (real and complex derivatives) (complete)
- [x] `DifferentialForm/` - Differential forms on normed spaces and exterior derivatives (complete)
- [x] `FDeriv/` - Fréchet derivatives (multivariable derivatives in normed spaces) (complete)
- [x] `Gradient/` - Gradient of functions (vector of partial derivatives in inner product spaces) (complete)
- [x] `InverseFunctionTheorem/` - Inverse function theorem (local invertibility from invertible derivative) (complete)
- [x] `IteratedDeriv/` - Iterated derivatives (nth derivatives) (complete)
- [x] `LineDeriv/` - Directional derivatives (derivatives along lines/vectors) (complete)
- [x] `LocalExtr/` - Local extrema and critical points (Fermat's theorem) (complete)
- [x] `TangentCone/` - Tangent cones and normal cones for convex analysis and optimization (complete)

## Search Tags

calculus differential-calculus derivatives fréchet-derivative directional-derivative iterated-derivative mean-value-theorem implicit-function-theorem inverse-function-theorem taylor-theorem lhopital darboux rademacher lagrange-multipliers parametric-integrals smooth-series uniform-convergence monotone-differentiability derivative-tests vector-fields lie-bracket formal-multilinear-series bump-functions conformal-maps continuously-differentiable local-extrema tangent-cone gradient slope
