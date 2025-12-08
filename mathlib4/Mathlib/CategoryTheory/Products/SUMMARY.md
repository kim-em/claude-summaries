---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Products
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 4
subdirs_count: 0
---

# Products

## Overview

The `Products/` directory provides the formalization of Cartesian product categories and functors between them. It defines the product category construction `C × D` with pointwise morphisms, fundamental projection and section functors (`fst`, `snd`, `sectL`, `sectR`), the swap equivalence showing products are symmetric, and evaluation functors for currying/uncurrying. The directory also includes coherence isomorphisms (associator and left/right unitors) establishing that product categories form a monoidal structure, along with specialized lemmas for bifunctors (functors out of product categories).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core product category instance `C × D` with morphism composition, projection/section functors (`fst`, `snd`, `sectL`, `sectR`), swap equivalence, evaluation functors, products of functors/natural transformations, and equivalence between `(A ⥤ B) × (A ⥤ C)` and `A ⥤ B × C` |
| Associator.lean | Associator equivalence `(C × D) × E ≌ C × (D × E)` with forward/inverse functors and compatibility with functor product conversions |
| Unitor.lean | Left and right unitor equivalences `Discrete PUnit × C ≌ C` and `C × Discrete PUnit ≌ C` establishing unit laws for product categories |
| Bifunctor.lean | Specialized lemmas for functors `F : C × D ⥤ E` including simplified `map_id`, diagonal interchange laws, and composition rules for bifunctors |

## Subdirectories

*(No subdirectories)*

## Search Tags

product-categories cartesian-product functors projections evaluation bifunctors associator unitor monoidal-structure currying swap-equivalence natural-transformations
