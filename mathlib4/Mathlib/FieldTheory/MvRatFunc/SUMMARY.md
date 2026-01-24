---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/MvRatFunc
generated: 2026-01-24T22:43:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# MvRatFunc

## Overview

The `MvRatFunc/` directory contains theory about multivariate rational function fields. It establishes the rank (vector space dimension over the base field) of the field of fractions of a multivariate polynomial ring. The main result shows that the rank equals the supremum of the cardinalities of the base field, the index set, and the countable cardinal ℵ₀.

## Key Files

| File | Purpose |
|------|---------|
| Rank.lean | Proves `MvRatFunc.rank_eq_max_lift`: the module rank of `FractionRing (MvPolynomial σ F)` over `F` equals `lift #F ⊔ lift #σ ⊔ ℵ₀` by showing upper bounds via cardinality and lower bounds via transcendental elements |

## Subdirectories

(No subdirectories)

## Search Tags

multivariate-rational-functions fraction-field multivariate-polynomials module-rank vector-space-dimension cardinality transcendental-elements field-theory
