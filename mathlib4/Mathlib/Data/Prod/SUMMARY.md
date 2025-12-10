---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Prod
generated: 2025-12-11T07:15:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 4
subdirs_count: 0
---

# Prod

## Overview

This directory provides the API for product types (`α × β`) in Mathlib. It includes basic lemmas and operations on pairs (swap, map, projections), lexicographic ordering on products with preorder/partial order/linear order instances, polymorphic dependent product `PProd`, and finite products over lists (`TProd`). The lexicographic order `α ×ₗ β` is used for well-founded induction and dictionary-style comparisons.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core lemmas about `Prod`: swap properties, map operations, projection injectivity/surjectivity, lexicographic relation basics, custom delaborators for `.1`/`.2` notation |
| Lex.lean | Lexicographic order instances for product types: `α ×ₗ β` notation, preorder, partial order, linear order, `OrderBot`/`OrderTop`/`BoundedOrder`, `DenselyOrdered`, `NoMaxOrder`/`NoMinOrder` |
| PProd.lean | Lemmas for `PProd` (universe-polymorphic dependent pairs): eta, forall/exists rewriting, injective map |
| TProd.lean | Finite products over lists (`List.TProd`): equivalence between `∀ i, α i` and iterated binary products when list contains all indices; used as intermediary for finitary product measures |

## Subdirectories

*(none)*

## Search Tags

product-types pairs tuples lexicographic-order prod-lex fst snd swap map pprod tprod finitary-products well-founded
