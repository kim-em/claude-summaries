---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/IteratedDeriv
generated: 2025-12-04T08:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# IteratedDeriv

## Overview

The `IteratedDeriv/` directory formalizes iterated derivatives (nth derivatives) for one-dimensional functions. It defines `iteratedDeriv n f` and `iteratedDerivWithin n f s` as the nth derivative obtained by applying the derivative operation n times, implemented via iterated Fréchet derivatives. The directory includes basic properties, algebraic operations (addition, scalar multiplication, composition), Faà di Bruno's formula for derivatives of compositions, convergence results connecting Taylor series to analytic functions on balls, and specialized results for power functions within open sets.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of `iteratedDeriv` and `iteratedDerivWithin` as evaluations of iterated Fréchet derivatives; proves equivalence to iterating the derivative operator (`iteratedDeriv_eq_iterate`), basic properties (0th derivative equals function, 1st derivative equals `deriv`), and characterization of C^n smoothness in terms of continuity and differentiability of iterated derivatives |
| Lemmas.lean | Algebraic operations on iterated derivatives requiring additional imports: linearity (`iteratedDerivWithin_add`, `iteratedDerivWithin_sub`), scalar multiplication (`iteratedDerivWithin_const_smul`, `iteratedDerivWithin_const_mul`), negation, composition with scaling (`iteratedDerivWithin_comp_const_smul`), translation invariance (`iteratedDeriv_comp_const_add`, `iteratedDeriv_comp_add_const`), and congruence results for functions equal on sets or eventually equal |
| FaaDiBruno.lean | Faà di Bruno's formula for iterated derivatives of compositions as sums over ordered finite partitions; includes specialized formulas for 2nd and 3rd derivatives of `(g ∘ f)` in three forms: `vcomp` for `g : E → F` with `f : 𝕜 → E`, `scomp` for `g : 𝕜 → E` with `f : 𝕜 → 𝕜`, and `comp` for scalar-valued compositions `g : 𝕜 → 𝕜` with `f : 𝕜 → 𝕜` |
| ConvergenceOnBall.lean | Proves that if a function `f : 𝕜 → 𝕜` is analytic on the ball of convergence of its Taylor series (defined via iterated derivatives `iteratedDeriv n f x / n.factorial`), then the series converges to `f` on that ball (`AnalyticOn.hasFPowerSeriesOnBall`); requires `RCLike 𝕜` to avoid pathological examples like p-adic indicator functions |
| WithinZpow.lean | Iterated derivatives of integer power functions `x ↦ x^m` (m : ℤ) within open sets; proves `iteratedDerivWithin k (y ↦ y^m) s = (∏ i < k, (m - i)) * y^(m - k)` and specialized formula for `1/y` involving factorials and powers of -1 |

## Subdirectories

(none)

## Search Tags

iterated-derivative nth-derivative one-dimensional-derivative derivative-iteration C-n-smoothness continuously-differentiable faa-di-bruno composition-derivatives chain-rule taylor-series analytic-functions power-series convergence-on-ball integer-powers zpow scalar-field normed-field
