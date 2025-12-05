---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/ContinuousFunctionalCalculus/ExpLog
generated: 2025-12-05T08:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# ExpLog

## Overview

The `ExpLog/` directory implements exponential and logarithm functions for operators, matrices, and C⋆-algebra elements via the continuous functional calculus (CFC). It defines `CFC.log` as the primary logarithm operation and proves that CFC-based exponentials coincide with power series exponentials (`NormedSpace.exp`). The directory provides API for both basic logarithm properties (identity, scalar multiplication, powers) and order-theoretic properties (monotonicity on strictly positive elements).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and API for CFC exponential and logarithm: proves `cfc Real.exp` equals `NormedSpace.exp`, defines `CFC.log` as `cfc Real.log`, provides basic properties (log of zero/one/algebraMap/smul/pow), and establishes log-exp inverse relationships |
| Order.lean | Order-theoretic properties of the operator logarithm: proves `CFC.log` is operator monotone on strictly positive elements using limit representation `log x = lim_{p → 0} p⁻¹(x^p - 1)` with locally uniform convergence |

## Subdirectories

*(No subdirectories)*

## Search Tags

continuous-functional-calculus cfc exponential logarithm operator-monotone strictly-positive cstar-algebra normed-space power-series inverse-functions selfadjoint order-theory operator-theory functional-analysis spectrum
