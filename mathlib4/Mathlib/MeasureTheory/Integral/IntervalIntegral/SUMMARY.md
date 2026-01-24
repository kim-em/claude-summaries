---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Integral/IntervalIntegral
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 10
subdirs_count: 0
---

# IntervalIntegral

## Overview

This directory contains the complete formalization of interval integration on ℝ using the notation `∫ x in a..b, f x`. It establishes both fundamental theorems of calculus (FTC-1 for derivatives of integrals, FTC-2 for integrals of derivatives), integration techniques (by parts, change of variables), and specialized results including the trapezoidal rule for numerical integration, the Lebesgue differentiation theorem for interval integrals, mean value theorems, and theory for periodic functions. The interval integral is defined as `∫ x in Ioc a b, f x ∂μ - ∫ x in Ioc b a, f x ∂μ` to avoid conditionals while ensuring additivity.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Foundation for interval integration: defines `IntervalIntegrable f μ a b` (integrable on both `Ioc a b` and `Ioc b a`), `∫ x in a..b, f x ∂μ` notation, basic properties (linearity, additivity, reversal, monotonicity), integration on subintervals, and interactions with continuity |
| FundThmCalculus.lean | Fundamental theorems of calculus for interval integrals: FTC-1 (derivatives of `(u,v) ↦ ∫ x in u..v, f x` in terms of boundary values), FTC-2 (integral of derivative equals endpoint difference), includes one-sided derivatives via `FTCFilter` typeclass, versions for locally finite measures, and specialized versions for right/left derivatives |
| IntegrationByParts.lean | Integration by parts and change of variables: proves `∫ x in a..b, u'x * vx + ux * v'x = ub * vb - ua * va` (product rule integration), `∫ x in a..b, (f ∘ g) x * g' x = ∫ y in g(a)..g(b), f y` (substitution), with versions for different derivative conditions (HasDerivAt, HasDerivWithinAt, HasDerivRight) |
| Periodic.lean | Integration of periodic functions: proves `Ioc t (t + T)` is fundamental domain for action of `ℤ ∙ T` on ℝ, establishes measure-preserving property of quotient map to AddCircle, proves `∫ x in t..t+T, f x = ∫ x in s..s+T, f x` for T-periodic functions, connects Lebesgue measure on intervals to Haar measure on the circle |
| TrapezoidalRule.lean | Numerical integration via trapezoidal rule: defines `trapezoidal_integral f N a b` (sum of N trapezoids with N+1 function evaluations), proves error bound in terms of second derivative bound, includes symmetry properties and subdivision formulas for composite trapezoidal integration |
| MeanValue.lean | First mean value theorem for interval integrals: proves existence of `c ∈ uIcc a b` such that `∫ x in a..b, f x * g x ∂μ = f c * ∫ x in a..b, g x ∂μ` when f is continuous and g is non-negative, with versions for both pointwise and almost everywhere non-negativity of g |
| ContDiff.lean | FTC for continuously differentiable functions: proves `∫ x in a..b, deriv f x = f b - f a` when f is C¹ on `[a,b]`, provides simpler interface than general FTC-2 for the common case of smooth functions, includes versions for both `deriv` and `derivWithin` |
| DerivIntegrable.lean | Integrability of derivatives for special function classes: proves `f'` is interval integrable when f is monotone on `a..b`, when f has bounded variation, or when f is absolutely continuous, includes bounds on `∫ f'` in terms of function variation (e.g., `∫ f' ∈ uIcc 0 (fb - fa)` for monotone f) |
| LebesgueDifferentiationThm.lean | Lebesgue differentiation for interval integrals: proves that for locally integrable f, almost every x satisfies `HasDerivAt (fun x => ∫ t in c..x, f t) (f x) x` for any c, with local version for interval integrability stating the same for almost every x in the interval |
| Slope.lean | Integration of slope functions: proves interval integrability of `fun x ↦ slope f x (x + c)` when f is interval integrable or monotone on appropriate intervals, establishes bound `∫ slope f x (x+c) ≤ f(b+c) - f(a)` for monotone f, foundational for derivative integrability results |

## Subdirectories

(No subdirectories)

## Search Tags

interval-integral interval-integrable fundamental-theorem-calculus ftc ftc-1 ftc-2 integration-by-parts change-of-variables substitution periodic-functions trapezoidal-rule numerical-integration mean-value-theorem lebesgue-differentiation-theorem monotone-functions bounded-variation absolutely-continuous slope derivative-integrability haar-measure additive-circle one-sided-derivatives continuously-differentiable
