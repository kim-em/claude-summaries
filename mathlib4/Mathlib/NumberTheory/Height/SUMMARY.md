---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/Height
generated: 2026-01-25T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 2
subdirs_count: 0
---

# Height

## Overview

The `Height/` directory formalizes height functions in Diophantine geometry, providing a general framework for multiplicative and logarithmic heights on fields equipped with families of absolute values satisfying the product formula. The implementation is designed to work across diverse contexts including algebraic number fields and function fields, and includes both element heights and projective heights for tuples.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core height theory defining `AdmissibleAbsValues` type class, multiplicative/logarithmic heights for field elements (`mulHeight₁`, `logHeight₁`) and tuples (`mulHeight`, `logHeight`), including fundamental properties like scaling invariance and power laws |
| Instances.lean | Concrete instance of `AdmissibleAbsValues` for algebraic number fields using infinite places (archimedean) and finite places (non-archimedean), with explicit formulas for heights in number fields |

## Subdirectories

*(No subdirectories)*

## Search Tags

height-functions diophantine-geometry absolute-values product-formula number-fields projective-space logarithmic-height multiplicative-height admissible-absolute-values archimedean non-archimedean infinite-places finite-places field-height
