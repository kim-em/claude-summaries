---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/Pow
generated: 2025-12-07T00:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 8
subdirs_count: 0
---

# Pow

## Overview

The `Pow/` directory provides comprehensive formalization of power functions `x^y` across different number systems (complex `ℂ`, real `ℝ`, nonnegative real `ℝ≥0`, extended nonnegative real `ℝ≥0∞`). It includes definitions, basic algebraic properties, continuity results, differentiability theorems, asymptotic behavior analysis, and integration formulas. The power function for complex numbers is defined as `x^y = exp(y log x)` with special handling for `x = 0`. Real powers inherit from complex powers by taking the real part, with additional complications for negative bases. The directory establishes a complete calculus framework for power functions, including strict derivatives, Fréchet derivatives, continuity at various points, and asymptotic comparisons with exponentials.

## Key Files

| File | Purpose |
|------|---------|
| Real.lean | Defines real power function `x^y` as real part of complex power; handles positive, zero, and negative bases with different formulas |
| Complex.lean | Defines complex power function `x^y = exp(y log x)` with special cases for zero; includes algebraic identities and inversion formulas |
| NNReal.lean | Nonnegative real powers `ℝ≥0 ^ ℝ` as restriction of real powers; includes algebraic properties and power laws |
| Continuity.lean | Continuity results for power functions on `ℂ`, `ℝ`, `ℝ≥0`, `ℝ≥0∞`; handles continuity at zero for positive exponents and slitPlane conditions |
| Deriv.lean | Derivatives and differentiability for power functions; includes `deriv (x^p) = p * x^(p-1)` and two-variable derivatives with logarithmic terms |
| Asymptotics.lean | Asymptotic behavior and limits at infinity; proves `x^s = o(exp(x))` and `log^r = o(x^s)` with IsBigO/IsLittleO notation |
| Integral.lean | Layer cake formula for integrals of power functions: `∫ f^p = p * ∫ t^(p-1) * μ{f ≥ t} dt` for nonnegative functions |
| NthRootLemmas.lean | Properties of natural number nth roots; proves `Nat.nthRoot n a` is floor of `ⁿ√a` with tightness bounds |

## Subdirectories

_(None)_

## Search Tags

power-functions rpow cpow complex-powers real-powers nonnegative-powers exponential logarithm continuity differentiability derivatives asymptotics limits big-o little-o integration layer-cake-formula nth-root floor-function slitplane fréchet-derivative strict-derivative power-laws algebraic-identities
