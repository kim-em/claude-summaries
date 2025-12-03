---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring/Action/Pointwise
generated: 2025-12-01T21:35:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Pointwise

## Overview

The `Pointwise/` directory provides properties of pointwise scalar actions and operations on sets and finite sets within rings and modules. It focuses on how negation interacts with scalar multiplication in the pointwise setting, establishing simplification lemmas like `-a • t = -(a • t)` for both sets and finite sets. These results extend the general pointwise operations framework to ring-theoretic contexts.

## Key Files

| File | Purpose |
|------|---------|
| Set.lean | Pointwise scalar actions on sets in modules over rings: negation compatibility `neg_smul_set`, `smul_set_neg`, and `add_smul_subset` for distributivity |
| Finset.lean | Pointwise scalar actions on finite sets: `neg_smul_finset` lemma showing negation commutes with scalar multiplication on finite sets |

## Subdirectories

None.

## Search Tags

pointwise-operations pointwise-scalar-action set-operations finset-operations scalar-multiplication negation module-action ring-module distributive-action pointwise-addition pointwise-multiplication
