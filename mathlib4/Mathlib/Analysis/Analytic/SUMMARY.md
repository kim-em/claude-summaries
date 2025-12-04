---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Analytic
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 19
subdirs_count: 0
---

# Analytic

## Overview

The `Analytic/` directory contains the formalization of analytic functions—functions that can be locally represented as converging power series. This is the foundation for complex analysis and smooth analysis in infinite dimensions. The directory provides a complete theory of power series expansions in arbitrary normed spaces, including existence, uniqueness, composition, inversion, and change of origin operations. It covers both classical results (isolated zeros principle, identity theorem) and modern developments (continuously polynomial functions, analytic functions on open partial homeomorphisms).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and basic properties of analytic functions; defines `HasFPowerSeriesOnBall`, `HasFPowerSeriesAt`, `AnalyticAt`, `AnalyticOnNhd`, and their "within" variants for functions with power series expansions; establishes continuity of functions admitting power series |
| ConvergenceRadius.lean | Theory of radius of convergence for formal power series; characterizes the largest ball on which a power series converges |
| Composition.lean | Proves composition of analytic functions is analytic via the formula `(g ∘ f)(y) = ∑ qₙ(p_{i₁}(y,...,y),...,p_{iₙ}(y,...,y))` over all compositions `i₁+...+iₙ=N`; includes associativity of formal composition |
| Constructions.lean | Algebraic operations on analytic functions (addition, multiplication, scalar multiplication, negation, subtraction); proves these preserve analyticity |
| ChangeOrigin.lean | Changing the center of a power series expansion; proves that if `f` is analytic in disk `D(x,R)` then it's analytic at any `y` in that disk, with series `p.changeOrigin y`; establishes that the set of points where a function is analytic is open |
| Inverse.lean | Construction and properties of formal left and right inverses of multilinear series with invertible linear term; proves they coincide and have positive radius when original series does; shows inverse of analytic open partial homeomorphism is analytic |
| Linear.lean | Proves continuous linear maps are analytic with power series `f(x) = f(a) + f(x-a)`; shows linear maps are continuously polynomial (admit finite power series) |
| Binomial.lean | Binomial-type expansions for analytic functions |
| CPolynomial.lean | Continuously polynomial functions (functions with finite power series expansions) |
| CPolynomialDef.lean | Definitions for continuously polynomial functions and their basic properties |
| IsolatedZeros.lean | Principle of isolated zeros for analytic functions of one variable; proves `AnalyticAt.eventually_eq_zero_or_eventually_ne_zero` (zeros are isolated or function is identically zero); includes identity theorem `AnalyticOnNhd.eqOn_of_preconnected_of_frequently_eq` |
| IteratedFDeriv.lean | Relationship between power series coefficients and iterated derivatives; establishes that analytic functions are infinitely differentiable |
| Order.lean | Order of vanishing for analytic functions at a point |
| Polynomial.lean | Proves polynomial evaluation is analytic; shows `aeval` of polynomials preserves analyticity |
| Uniqueness.lean | Uniqueness results for analytic functions (identity theorem variants) |
| Within.lean | Analytic functions on subsets; defines `AnalyticWithinAt` and `AnalyticOn` for convergence restricted to a set |
| WithLp.lean | Analytic functions on Lp spaces |
| OfScalars.lean | Building analytic functions from scalar-valued analytic functions |
| RadiusLiminf.lean | Computing radius of convergence via liminf formula |

## Subdirectories

(none)

## Search Tags

analytic-functions power-series formal-multilinear-series convergence-radius composition inverse change-origin isolated-zeros identity-theorem polynomial continuously-polynomial binomial iterated-derivatives holomorphic complex-analysis infinite-dimensional-analysis banach-spaces normed-spaces complete-spaces
