---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/Complex
generated: 2025-12-05T08:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 9
subdirs_count: 0
---

# Complex

## Overview

The `Complex/` directory contains formalized theory for complex-valued special functions and their analytical properties. It focuses on the complex logarithm, argument function, arctangent, and their applications to the unit circle and additive characters. The directory provides detailed differentiability results, continuity properties, integral representations, Taylor series, bounds, homeomorphisms between the circle and real/additive circles, and connections to roots of unity. Key topics include the slit plane (ℂ \ ℝ≤0), arg as a multi-valued function normalized to (-π, π], log with principal branch, and various parameterizations of the unit circle.

## Key Files

| File | Purpose |
|------|---------|
| Analytic.lean | Proves log, cpow (complex power), and Real.log are analytic away from the slit plane; composition and restriction results for analyticity |
| Arctan.lean | Complex arctangent function defined via complex logarithm; proves tan(arctan z) = z and arctan(tan z) = z; includes power series expansion valid on open unit disc |
| Arg.lean | Argument function arg : ℂ → ℝ returning values in (-π, π]; proves sin(arg x) = x.im/‖x‖ and cos(arg x) = x.re/‖x‖; includes continuity on slit plane and angle arithmetic |
| Circle.lean | Maps on unit circle: expMapCircle and arg restricted to circle form partial equivalence; proves Circle.exp and Circle.argEquiv homeomorphism; includes Real.Angle.toCircle and AddCircle.toCircle |
| CircleAddChar.lean | Additive characters valued in unit circle from ZMod N and AddCircle T; proves primitivity of stdAddChar and connections to roots of unity |
| CircleMap.lean | Parameterization circleMap c R : ℝ → ℂ defined as θ ↦ c + R·exp(θi); proves injectivity on intervals, periodicity, and membership in spheres |
| Log.lean | Complex logarithm log : ℂ → ℂ with principal branch (im ∈ (-π, π]); proves exp(log x) = x and log(exp x) = x under branch conditions; includes log multiplication, inversion, and continuity results |
| LogBounds.lean | Estimates for log(1+z) - Taylor polynomials: ‖log(1+z) - Σ(-1)^(n+1)z^n/n‖ ≤ ‖z‖^(n+1)/((n+1)(1-‖z‖)); integral representation of log; Taylor series convergence on unit disc; limits of (1 + t/x)^x as x → ∞ |
| LogDeriv.lean | Differentiability of complex log: hasStrictDerivAt log x⁻¹ on slit plane; composition results for log derivatives; proves deriv(log ∘ f) = logDeriv f; includes expPartialHomeomorph |

## Subdirectories

(none)

## Search Tags

complex-analysis logarithm argument slit-plane arctangent unit-circle circle-map additive-characters roots-of-unity analytic-functions differentiability Taylor-series integral-representation homeomorphisms ZMod-characters AddCircle exp-map arg-function principal-branch continuity limits asymptotic-expansions special-functions
