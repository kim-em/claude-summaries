---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/ContinuousFunctionalCalculus/PosPart
generated: 2025-12-05T07:10:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# PosPart

## Overview

The `PosPart/` directory defines the positive and negative parts of selfadjoint elements in C⋆-algebras via the continuous functional calculus (CFC). For a selfadjoint element `a`, the positive part `a⁺ = max(a, 0)` and negative part `a⁻ = max(-a, 0)` satisfy `a = a⁺ - a⁻` and `a⁺ * a⁻ = 0`. The implementation provides both non-unital and unital versions, proves uniqueness of the decomposition, establishes norm relationships (`‖a‖ = max ‖a⁺‖ ‖a⁻‖`), and demonstrates that C⋆-algebras are spanned by their nonnegative elements.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core positive/negative part API including definitions via `cfcₙ`, uniqueness theorem (`posPart_negPart_unique`), algebraic properties (orthogonality, scalar multiplication, negation), order relationships, and proof that C⋆-algebras are spanned by nonnegative elements |
| Isometric.lean | Norm properties of positive/negative parts in isometric CFC setting, proving `‖a⁺‖ ≤ ‖a‖`, `‖a⁻‖ ≤ ‖a‖`, and `‖a‖ = max ‖a⁺‖ ‖a⁻‖` for selfadjoint elements |

## Subdirectories

*(No subdirectories)*

## Search Tags

positive-part negative-part pospart negpart selfadjoint cstar-algebra continuous-functional-calculus cfc decomposition jordan-decomposition orthogonal nonnegative uniqueness norm-bounds isometric spectral-theory functional-analysis max-function star-ordered-ring star-algebra
