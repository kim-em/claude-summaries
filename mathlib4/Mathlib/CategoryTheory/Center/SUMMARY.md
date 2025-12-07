---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Center
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Center

## Overview

The `Center/` directory formalizes the center of a category, defined as `CatCenter C := End (𝟭 C)`, the endomorphisms of the identity functor. This structure forms a commutative monoid where elements act on morphisms and objects via scalar multiplication, generalizing the notion of central elements from algebra to category theory. The formalization includes specialized results for preadditive categories (where the center gains additive structure), linear categories (with ring morphisms `R →+* CatCenter C`), and localization (functorial behavior under localization functors).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `CatCenter C` as endomorphisms of identity functor with naturality, multiplication commutativity, and scalar multiplication on morphisms and isomorphisms |
| Preadditive.lean | Additive structure on `CatCenter C` for preadditive categories with lemmas for `app_add`, `app_sub`, `app_neg` |
| Linear.lean | Ring morphism `R →+* CatCenter C` for linear categories and construction of linear structure from such morphisms |
| Localization.lean | Localization map `CatCenter C → CatCenter D` for localization functors, promoted to ring morphism `CatCenter C →+* CatCenter D` for additive functors |

## Subdirectories

*(No subdirectories)*

## Search Tags

category-theory center endomorphisms identity-functor natural-transformations commutative-monoid scalar-multiplication preadditive linear-categories localization ring-morphisms
