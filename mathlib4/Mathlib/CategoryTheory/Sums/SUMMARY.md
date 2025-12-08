---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Sums
generated: 2025-12-08T15:47:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# Sums

## Overview

The `Sums/` directory formalizes binary disjoint unions (coproducts) of categories, providing the category structure on `C ⊕ D`, functors between sum categories, and universal properties. It defines the canonical inclusion functors `inl_` and `inr_`, swap functors with equivalence proofs, associators establishing `(C ⊕ D) ⊕ E ≌ C ⊕ (D ⊕ E)`, and the universal property characterizing functors out of sums as equivalent to products of functors `A ⊕ A' ⥤ B ≌ (A ⥤ B) × (A' ⥤ B)`. This provides the categorical dual to the product constructions, enabling coproduct reasoning in category theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Binary disjoint union category instance on `C ⊕ D` with inclusion functors `inl_` and `inr_`, swap functor and equivalence, sum of functors `F.sum' G`, induction principle `Sum.homInduction`, and natural transformations on sums |
| Associator.lean | Associator functor `(C ⊕ D) ⊕ E ⥤ C ⊕ (D ⊕ E)` and inverse establishing equivalence `associativity`, characterizing compositions with inclusions |
| Products.lean | Universal property of sums as equivalence `Sum.functorEquiv : A ⊕ A' ⥤ B ≌ (A ⥤ B) × (A' ⥤ B)` with characterizations of compositions with projections and inclusions, compatibility with swap and associator |

## Subdirectories

(none)

## Search Tags

category-theory coproducts disjoint-union sum-categories inclusion-functors swap-functor associator universal-property functor-categories equivalences categorical-duality
