---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/PSigma
generated: 2025-12-11T22:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 0
---

# PSigma

## Overview

This folder provides lexicographic ordering for `PSigma` (dependent pair types with flexible universe polymorphism). It defines the type synonym `Σₗ' i, α i` for sigma types equipped with lexicographic order, where pairs are compared first by their index and then by their values within the same index. The file provides order-theoretic instances (preorder, partial order, linear order) and establishes properties like density, boundedness, and the existence of elements without maximum/minimum.

## Key Files

| File | Purpose |
|------|---------|
| Order.lean | Lexicographic order on `PSigma` types: defines `Σₗ' i, α i` notation, provides Preorder/PartialOrder/LinearOrder instances, and proves OrderBot/OrderTop/BoundedOrder/DenselyOrdered/NoMaxOrder/NoMinOrder instances under appropriate conditions |

## Subdirectories

None.

## Search Tags

psigma dependent-pairs sigma-types lexicographic-order lex-order preorder partial-order linear-order bounded-order densely-ordered universe-polymorphism
