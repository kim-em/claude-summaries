---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/FreeAlgebra
generated: 2025-12-01T10:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# FreeAlgebra

## Overview

This folder contains cardinality theory for free algebras, specifically analyzing the cardinality of `FreeAlgebra R X` in terms of the cardinalities of the base semiring `R` and the generator type `X`. The results are parallel to cardinality results for `MvPolynomial` and establish tight bounds for the size of free algebras under various conditions (nontrivial/subsingleton, empty/nonempty generators).

## Key Files

| File | Purpose |
|------|---------|
| Cardinality.lean | Proves cardinality theorems for `FreeAlgebra R X`: main result is `#(FreeAlgebra R X) = lift #R ⊔ lift #X ⊔ ℵ₀` for nontrivial R and nonempty X, with specialized results for empty generators and subsingleton base rings; also bounds cardinality of `Algebra.adjoin R s` |

## Subdirectories

(none)

## Search Tags

free-algebra cardinality cardinal set-theory infinite algebra generators polynomial monoid-algebra finsupp
