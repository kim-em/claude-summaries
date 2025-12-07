---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Enriched
generated: 2025-12-07T12:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 6
subdirs_count: 2
---

# Enriched

## Overview

The `Enriched/` directory contains the formalization of enriched category theory in mathlib4, where categories are enriched over a monoidal category `V`. Unlike ordinary categories where morphisms form sets, enriched categories have hom-objects in `V`, with composition given by morphisms in `V` satisfying coherence conditions. This framework generalizes ordinary category theory (enrichment over `Type`), metric spaces (enrichment over `[0,∞]`), and 2-categories (enrichment over `Cat`). The directory provides the basic theory of `V`-enriched categories, enriched functors, enriched natural transformations, and shows these structures reduce to ordinary categories when `V = Type`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `V`-enriched categories, `V`-functors, enriched natural transformations, and proof that `Type v`-enriched categories coincide with ordinary categories |
| EnrichedCat.lean | Bundled `V`-enriched categories and bicategory structure on `EnrichedCat V` with whiskering operations and coherence isomorphisms |
| FunctorCategory.lean | Enrichment of functor categories `J ⥤ C` when `C` is `V`-enriched, defining enriched hom objects as ends and proving functor categories are both `V`-enriched and `J ⥤ V`-enriched |
| HomCongr.lean | Isomorphisms between enriched hom-objects induced by isomorphisms of domain/codomain, parallel to `HomCongr` for ordinary categories |
| Opposite.lean | Construction of opposite `V`-category for braided monoidal `V`, using the braiding to define composition, and equivalence between underlying categories |

## Subdirectories

- [x] `Limits/` - Conical limits in enriched categories (complete)
- [x] `Ordinary/` - Enriched ordinary categories with compatibility between enriched and ordinary structure (complete)

## Search Tags

enriched-categories monoidal-categories enriched-functors enriched-natural-transformations functor-categories ends opposite-category braided-monoidal enriched-homs bicategory-structure category-theory type-enrichment ordinary-categories underlying-categories
