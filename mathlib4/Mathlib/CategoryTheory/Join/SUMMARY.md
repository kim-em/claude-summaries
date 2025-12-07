---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Join
generated: 2025-12-07T08:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# Join

## Overview

The `Join/` directory formalizes the join construction for categories, denoted `C ⋆ D`. The join of categories `C` and `D` creates a new category whose objects are disjoint unions of `C` and `D`, preserving morphisms within each category while adding a unique morphism from every object in `C` to every object in `D`. This construction is foundational in higher category theory and appears in the theory of simplicial sets and ∞-categories. The directory provides comprehensive API including functor constructors, natural transformation builders, opposites, pseudofunctoriality as a bifunctor on Cat, (co)finality properties, and embeddings from categorical sums.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core join construction defining `C ⋆ D` with objects `left c` and `right d`, canonical inclusions `inclLeft` and `inclRight`, unique edge morphisms `edge c d`, functor constructor `mkFunctor`, natural transformation constructor `mkNatTrans`, `mapPair` for functoriality, and equivalence preservation |
| Final.lean | (Co)finality properties: `inclLeft C D` is initial when `C` is connected, `inclRight C D` is final when `D` is connected, with equivalences between structured/costructured arrow categories and base categories |
| Opposites.lean | Canonical equivalence `(C ⋆ D)ᵒᵖ ≌ Dᵒᵖ ⋆ Cᵒᵖ` with characterization of both directions via the inclusions |
| Pseudofunctor.lean | Pseudofunctoriality of join as bifunctor on Cat: `pseudofunctorLeft D : Cat ⥤ Cat` and `pseudofunctorRight C : Cat ⥤ Cat` with coherence isomorphisms for composition, identities, associators, and unitors |
| Sum.lean | Canonical faithful essentially surjective functor `fromSum : C ⊕ D ⥤ C ⋆ D` embedding categorical sum into join, characterized via sum inclusions |

## Subdirectories

(No subdirectories)

## Search Tags

category-theory join-of-categories categorical-joins simplicial-categories higher-category-theory simplicial-sets infinity-categories initial-functors final-functors pseudofunctors bifunctors connected-categories costructured-arrows structured-arrows opposite-categories categorical-sums
