---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/Log
generated: 2025-12-05T07:00:00Z
git_sha: 9f4e7a48e4c91404feac52c10298674a9361184f
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 11
subdirs_count: 0
---

# Log

## Overview

The `Log/` directory provides comprehensive formalization of logarithm functions across multiple number systems: real logarithms (`Real.log`), logarithms in arbitrary bases (`Real.logb`), extended nonnegative real logarithms (`ENNReal.log` mapping to `EReal`), and extended real exponentials (`EReal.exp` mapping to `ℝ≥0∞`). The directory establishes core properties including continuity, differentiability, monotonicity, algebraic identities (log laws, exp-log inverses), asymptotic behavior, series expansions, and special function constructions like the positive part of logarithm and the Shannon-entropy-related function `-x * log x`. These results support analysis, information theory, probability, and measure theory applications throughout mathlib4.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Real logarithm definition and basic properties; defines `Real.log` with extension to all reals (log 0 = 0, log(-x) = log x); proves continuity, surjectivity, exp-log inverses, and fundamental inequalities |
| Base.lean | Logarithm in arbitrary base `b`; defines `Real.logb b x = log x / log b`; proves algebraic identities (logb_mul, logb_div, logb_inv), change of base formula, continuity, and differentiability |
| Deriv.lean | Derivatives and smoothness of real logarithm; proves `deriv log x = x⁻¹` for x ≠ 0, infinite differentiability at nonzero points, and series expansion `∑' n, x^(n+1)/(n+1) = -log(1-x)` for \|x\| < 1 |
| ENNRealLog.lean | Extended nonnegative real logarithm `ENNReal.log : ℝ≥0∞ → EReal` with `log 0 = ⊥`, `log ⊤ = ⊤`; proves strict monotonicity, injectivity, surjectivity, bijectivity, and identities `log(x*y) = log x + log y`, `log(x^n) = n * log x` |
| ENNRealLogExp.lean | Order isomorphisms and homeomorphisms between `ℝ≥0∞` and `EReal` via log and exp; defines `ENNReal.logOrderIso`, `EReal.expOrderIso`, `ENNReal.logHomeomorph`, `EReal.expHomeomorph`; proves `EReal` is a Polish space |
| ERealExp.lean | Extended real exponential `EReal.exp : EReal → ℝ≥0∞` with `exp ⊥ = 0`, `exp ⊤ = ⊤`; proves strict monotonicity and identities `exp(-x) = (exp x)⁻¹` and `exp(x+y) = exp x * exp y` |
| Monotone.lean | Monotonicity and antitonicity of logarithm multiplied by powers; proves `x ↦ log x * x` is monotone on [1,∞), `x ↦ log x / x` is antitone on [e,∞), and `x ↦ log x / x^a` is antitone on appropriate domains |
| NegMulLog.lean | The function `x ↦ -x * log x` used in Shannon entropy; proves continuity everywhere (including at zero via limit), differentiability on ℝ \ {0} with derivative `-(log x + 1)`, and asymptotic behavior |
| PosLog.lean | Positive part of logarithm `log⁺(x) = max(0, log x)` with notation `log⁺`; proves subadditivity estimates `log⁺(∏ f i) ≤ ∑ log⁺(f i)` and `log⁺(∑ f i) ≤ log n + ∑ log⁺(f i)` for finite sequences |
| RpowTendsto.lean | Logarithm as limit of powers; proves `p⁻¹ * (x^p - 1)` tends to `log x` as `p → 0` for positive `x`, with both pointwise and uniform convergence on compact subsets of (0,∞) |
| Summable.lean | Summability of logarithms and infinite products; proves summable logarithms imply multipliability, `exp(∑' log f i) = ∏' f i`, and `log(1 + f i)` summable when `f i` summable (for both real and complex) |

## Subdirectories

No subdirectories.

## Search Tags

logarithm log real-logarithm logarithm-base logb derivative continuity differentiability smooth infinite-differentiability series-expansion extended-nonnegative-real ennreal extended-real ereal exponential exp order-isomorphism homeomorphism polish-space monotonicity antitonicity tonality shannon-entropy neg-mul-log positive-part poslog power-limit rpow summability infinite-products multipliability exp-log-inverse log-laws algebraic-identities asymptotic-behavior
