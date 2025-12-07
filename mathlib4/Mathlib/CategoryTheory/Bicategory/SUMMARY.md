---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Bicategory
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 14
subdirs_count: 8
---

# Bicategory

## Overview

The `Bicategory/` directory provides a comprehensive formalization of bicategory theory in mathlib4. Bicategories are a fundamental weakening of 2-categories where composition of 1-morphisms is associative and unital only up to coherent isomorphisms rather than strict equalities. This directory implements the complete infrastructure for bicategorical reasoning, from the core definitions through advanced constructions and universal properties.

The directory includes the basic bicategory typeclass with 1-morphisms, 2-morphisms, left/right whiskering operations, associators, and unitors satisfying pentagon and triangle coherence axioms. It provides fundamental constructions including free bicategories over quivers (with a coherence theorem proving local thinness), locally discrete bicategories, opposite bicategories, product bicategories, and structures induced from Cat-enriched categories and monoidal categories.

The functor theory comprises a full hierarchy from prelax functors (minimal structure) through lax/oplax functors (with coherent natural transformations for identity and composition) to pseudofunctors (where these are isomorphisms) and strict pseudofunctors. Natural transformations are provided in three flavors (lax, oplax, strong) with modifications as 2-morphisms between them. The `FunctorBicategory/` subdirectory realizes oplax functors as a bicategory with transformations as 1-morphisms and modifications as 2-morphisms.

Advanced structures include adjunctions in bicategories with the mate correspondence (establishing bijections between 2-cells via conjugate equivalences), a bicategory of adjunctions where 1-morphisms are adjoint pairs, Kan extensions with universal properties characterized as initial objects in extension categories, and the fundamental theorem that adjunctions are precisely Kan extensions of the identity. Comonads are formalized as comonoid objects in endomorphism categories and shown equivalent to oplax functors from the trivial bicategory. The directory also provides specialized infrastructure for strict bicategories where coherence isomorphisms reduce to equalities, allowing ordinary categorical reasoning.

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

- [x] `Adjunction/` - Adjunctions in bicategories with unit, counit, mate correspondence, and bicategory of adjunctions
- [x] `Functor/` - Hierarchy of functors from prelax through lax/oplax to pseudofunctors and strict pseudofunctors
- [x] `FunctorBicategory/` - Bicategory structure on oplax functors with natural transformations and modifications
- [x] `Kan/` - Kan extensions and lifts with universal properties and relationship to adjunctions
- [x] `Modification/` - Modifications as 2-morphisms between natural transformations of functors
- [x] `Monad/` - Comonads in bicategories as comonoid objects, equivalence with oplax functors from trivial bicategory
- [x] `NaturalTransformation/` - Lax, oplax, and strong transformations for lax/oplax functors and pseudofunctors
- [x] `Strict/` - Strict bicategories with equality-based coherence and specialized functor API

## Search Tags

bicategory 2-category weak-2-category whiskering associator unitor coherence-theorem free-bicategory pseudofunctor lax-functor oplax-functor natural-transformation modification grothendieck-construction kan-extension adjunction monad locally-discrete cat-enriched monoidal-category bicategorical-limit
