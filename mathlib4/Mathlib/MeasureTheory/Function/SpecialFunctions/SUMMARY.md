---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function/SpecialFunctions
generated: 2026-01-25T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# SpecialFunctions

## Overview

The `SpecialFunctions/` directory establishes measurability properties for standard mathematical special functions in measure theory. This includes proofs that common real and complex functions (exponential, logarithm, trigonometric, hyperbolic, power functions, arctan, arcsin, arccos) are measurable, as well as measurability of inner products in inner product spaces and basic RCLike operations. The module also provides measurability and integrability results for the sinc function.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core measurability theorems for standard real and complex functions (exp, log, sin, cos, sinh, cosh, arcsin, arccos) and their compositions; includes MeasurablePow instances for ℂ, ℝ, ℝ≥0, and ℝ≥0∞ |
| Arctan.lean | Measurability of the arctan function for both direct use and composition with measurable functions |
| Inner.lean | Measurability of inner products in inner product spaces over RCLike fields, including const_inner and inner_const variants |
| RCLike.lean | Measurability of RCLike typeclass operations (re, im, ofReal) and reconstruction of measurable RCLike-valued functions from their real and imaginary parts |
| Sinc.lean | Measurability, strong measurability, and integrability properties of the sinc function with respect to finite measures |

## Subdirectories

*(No subdirectories)*

## Search Tags

measurable special-functions exponential logarithm trigonometric hyperbolic arctan arcsin arccos power-functions complex-analysis inner-product rclike sinc integrability composition-lemmas fun-prop
