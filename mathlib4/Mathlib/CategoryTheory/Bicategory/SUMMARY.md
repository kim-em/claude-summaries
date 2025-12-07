---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Bicategory
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 14
subdirs_count: 8
---

# Bicategory

## Overview

The `Bicategory/` directory contains the formalization of bicategory theory in mathlib4. Bicategories are a weakened form of 2-categories where composition of 1-morphisms is associative only up to coherent isomorphism (associators), with specified unitors for identity morphisms. The directory implements the core bicategory typeclass with whiskering operations, free bicategories over quivers, the coherence theorem, various bicategorical constructions (opposites, products, Grothendieck construction), and structures for working with pseudofunctors, modifications, natural transformations, adjunctions, and Kan extensions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core bicategory typeclass with 1-morphisms, 2-morphisms, whiskering, associators, and unitors |
| Free.lean | Free bicategory construction over a quiver with freely generated 1-morphisms and 2-morphisms |
| Coherence.lean | Coherence theorem: free bicategory over any quiver is locally thin (at most one 2-morphism between 1-morphisms) |
| LocallyDiscrete.lean | Locally discrete bicategories where 2-morphisms are only equalities between 1-morphisms |
| Opposites.lean | Opposite bicategory construction reversing 1-morphisms while preserving 2-morphism direction |
| Product.lean | Cartesian product of bicategories with projection and section pseudofunctors |
| Grothendieck.lean | Grothendieck and CoGrothendieck constructions for pseudofunctors to Cat |
| Extension.lean | Left and right extensions (Kan extensions) in bicategories via structured arrow categories |
| CatEnriched.lean | Strict bicategory structure from Cat-enriched categories with hom-categories |
| End.lean | Endomorphisms of an object in a bicategory as a monoidal category |
| SingleObj.lean | Promoting a monoidal category to a single-object bicategory |
| EqToHom.lean | Behavior of eqToHom 1-morphisms and 2-morphisms in bicategories with coherence isomorphisms |
| InducedBicategory.lean | Bicategory structure induced via a function on objects |
| Strict.lean | Import for strict bicategory constructions |

## Subdirectories

- [x] `Adjunction/` - Adjunctions in bicategories (complete)
- [x] `Functor/` - Pseudofunctors and related structures between bicategories (complete)
- [x] `FunctorBicategory/` - Bicategory of oplax functors with oplax natural transformations and modifications (complete)
- [x] `Kan/` - Kan extensions in bicategories (complete)
- [x] `Modification/` - Modifications between natural transformations of oplax/pseudofunctors (complete)
- [x] `Monad/` - Comonads in bicategories as comonoid objects in endomorphism categories (complete)
- [x] `NaturalTransformation/` - Natural transformations for pseudofunctors (complete)
- [x] `Strict/` - Strict bicategories and related structures (complete)

## Search Tags

bicategory 2-category weak-2-category whiskering associator unitor coherence-theorem free-bicategory pseudofunctor lax-functor oplax-functor natural-transformation modification grothendieck-construction kan-extension adjunction monad locally-discrete cat-enriched monoidal-category bicategorical-limit
