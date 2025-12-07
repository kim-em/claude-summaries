---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Enriched/Ordinary
generated: 2025-12-07T09:07:23Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# Ordinary

## Overview

The `Ordinary/` directory formalizes the bridge between enriched categories and ordinary categories. When a category `C` has both a standard `Category` instance and a `V`-enriched structure, the `EnrichedOrdinaryCategory V C` typeclass captures the compatibility condition: morphisms `X ⟶ Y` in `C` must correspond bijectively to morphisms `𝟙_ V ⟶ (X ⟶[V] Y)` in `V`. This reconciles the two perspectives and ensures the enriched structure genuinely extends the ordinary category structure. Every `V`-enriched category induces an ordinary category `ForgetEnrichment V C` which is canonically equipped with this compatibility.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `EnrichedOrdinaryCategory` typeclass requiring `homEquiv : (X ⟶ Y) ≃ (𝟙_ V ⟶ (X ⟶[V] Y))` compatible with composition, constructs enriched coyoneda bifunctor `Cᵒᵖ ⥤ C ⥤ V`, proves `ForgetEnrichment V D` is enriched ordinary, establishes equivalence between enriched ordinary categories and their forgetful categories, and shows enriched ordinary structure transports along lax monoidal functors and restricts to full subcategories |

## Subdirectories

*(none)*

## Search Tags

enriched-ordinary-categories enriched-categories monoidal-categories ordinary-categories forget-enrichment hom-equiv enriched-coyoneda transport-enrichment full-subcategories whiskering lax-monoidal-functors category-theory type-enrichment simplicial-categories compatibility-conditions
