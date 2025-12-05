---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/ContinuousFunctionalCalculus
generated: 2025-12-05T07:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 2
subdirs_count: 3
---

# ContinuousFunctionalCalculus

## Overview

The `ContinuousFunctionalCalculus/` directory defines special functions (absolute value, exponential, logarithm, real powers, positive/negative parts, square root) via the continuous functional calculus (CFC) for C⋆-algebras and star-ordered rings. This allows applying real-valued special functions to operators, matrices, and other algebraic structures while preserving continuity and spectral properties. The directory provides both unital (cfc) and non-unital (cfcₙ) versions of these functions, with API covering algebraic properties, order relationships, commutativity conditions, and connections to existing power series definitions.

## Key Files

| File | Purpose |
|------|---------|
| Abs.lean | Absolute value via CFC defined as `abs a := sqrt (star a * a)`; includes properties for star-normal elements, commutativity, nonnegative powers, and norm preservation in C⋆-algebras |
| ExpLog.lean | Deprecated module file that re-exports `ExpLog.Basic`; marks the module as deprecated since 2025-11-15 |

## Subdirectories

- [x] `ExpLog/` - Exponential and logarithm functions via CFC (complete)
- [x] `PosPart/` - Positive and negative parts of selfadjoint elements (complete)
- [x] `Rpow/` - Real powers and square root via CFC (complete)

## Search Tags

continuous-functional-calculus cfc special-functions cstar-algebra star-ordered-ring absolute-value exponential logarithm real-powers square-root positive-part negative-part selfadjoint operators matrices functional-analysis spectral-theory unital non-unital
