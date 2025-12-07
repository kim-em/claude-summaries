---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Idempotents
generated: 2025-12-07T20:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 8
subdirs_count: 0
---

# Idempotents

## Overview

This folder contains the formalization of idempotent complete categories (also known as Karoubian or pseudoabelian categories) and the Karoubi envelope construction. The core contribution is the Karoubi envelope functor `toKaroubi : C ⥤ Karoubi C`, which universally embeds any category into an idempotent complete category. When the target category is already idempotent complete, this functor becomes an equivalence. The folder includes applications to functor categories, homological complexes, and simplicial objects, showing that idempotent completeness is preserved under these constructions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `IsIdempotentComplete C` typeclass expressing that all idempotent endomorphisms split; proves abelian categories are idempotent complete; establishes equivalence-invariance and opposite-category duality |
| Karoubi.lean | Defines the Karoubi envelope `Karoubi C` as formal direct factors (objects with idempotent endomorphisms); constructs fully faithful functor `toKaroubi : C ⥤ Karoubi C` which is an equivalence when `C` is idempotent complete; proves `Karoubi C` is always idempotent complete and preadditive when `C` is |
| FunctorExtension.lean | Extends functors to the Karoubi envelope via equivalences `karoubiUniversal₁ : (C ⥤ Karoubi D) ≌ (Karoubi C ⥤ Karoubi D)`, `karoubiUniversal₂ : (C ⥤ D) ≌ (Karoubi C ⥤ Karoubi D)` (when `D` idempotent complete), and `karoubiUniversal : (C ⥤ D) ≌ (Karoubi C ⥤ D)` (when `D` idempotent complete) |
| Biproducts.lean | Shows `Karoubi C` has finite biproducts when `C` is additive; constructs canonical decomposition `P ⊞ P.complement ≅ (toKaroubi C).obj P.X` where `P.complement` is the formal direct factor given by `𝟙 P.X - P.p` |
| FunctorCategories.lean | Proves functor categories `J ⥤ C` are idempotent complete when `C` is; constructs fully faithful embedding `karoubiFunctorCategoryEmbedding : Karoubi (J ⥤ C) ⥤ (J ⥤ Karoubi C)` sending formal direct factors componentwise |
| KaroubiKaroubi.lean | Establishes the idempotence of Karoubi envelope via equivalence `Karoubi C ≌ Karoubi (Karoubi C)`, showing that applying the Karoubi construction twice yields nothing new |
| HomologicalComplex.lean | Constructs equivalence `Karoubi (HomologicalComplex C c) ≌ HomologicalComplex (Karoubi C) c` commuting Karoubi envelope with homological complex formation; proves `HomologicalComplex C c` is idempotent complete when `C` is; includes specialized versions for chain and cochain complexes |
| SimplicialObject.lean | Provides instances showing `SimplicialObject C` and `CosimplicialObject C` are idempotent complete when `C` is, by applying the functor category idempotent completeness result |

## Subdirectories

(none)

## Search Tags

idempotent-complete karoubi-envelope pseudoabelian karoubian-category formal-direct-factors split-idempotents functor-extension homological-algebra simplicial-objects additive-categories preadditive-categories biproducts universal-property category-equivalence
