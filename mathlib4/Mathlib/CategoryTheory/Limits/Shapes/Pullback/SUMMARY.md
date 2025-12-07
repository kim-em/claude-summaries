---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Shapes/Pullback
generated: 2025-12-07T15:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 13
subdirs_count: 1
---

# Pullback

## Overview

The `Pullback/` directory provides an extended theory of pullbacks (and dually, pushouts) in category theory, building on the basic pullback/pushout API defined in the parent `Shapes/` directory. It includes core definitions (cospan/span diagrams, pullback cones, HasPullback typeclass), properties of pullbacks (pasting lemmas, associativity, interactions with monomorphisms/isomorphisms), commutative square formulations (IsPullback/IsPushout predicates), special cases (equalizers as pullbacks), and categorical/2-categorical perspectives (categorical pullbacks in the (2,1)-categorical sense with functors and natural transformations). This directory serves as the comprehensive reference for working with pullback diagrams beyond the basic universal property.

## Key Files

| File | Purpose |
|------|---------|
| Cospan.lean | Defines WalkingCospan and WalkingSpan indexing categories, with cospan/span functors for building pullback/pushout diagrams |
| PullbackCone.lean | API for pullback cones (resp. pushout cocones): PullbackCone.mk constructor, universal properties, morphisms between cones |
| HasPullback.lean | HasPullback typeclass and pullback/pushout API: pullback.fst, pullback.snd, pullback.lift with universal properties |
| Pasting.lean | Pasting lemmas for pullbacks: composing adjacent pullback squares, pasteHorizIsPullback, leftSquareIsPullback, and API isomorphisms |
| CommSq.lean | IsPullback and IsPushout predicates for commutative squares, bi-Cartesian squares, and interconversion with IsLimit API (1700+ lines) |
| Mono.lean | Interactions between pullbacks and monomorphisms: stability under pullback, composition with monomorphisms preserves limits, kernel pairs |
| Iso.lean | Pullbacks and pushouts of isomorphisms: explicit limit cones showing pullback of iso is iso to the other leg |
| Assoc.lean | Associativity of pullbacks: natural isomorphisms showing (W ×[Y] X) ×[Z] Y ≅ W ×[Y] (X ×[Z] Y) |
| Square.lean | Translation of IsPullback/IsPushout API to Square C category of commutative squares, with stability of mono/epi properties |
| Connected.lean | Pullbacks commute with connected limits: isLimitOfIsPullbackOfIsConnected showing limits of pullback diagrams |
| Equalizer.lean | Equalizers as pullbacks: shows equalizer of f,g is pullback of diagonal Y → Y×Y along (f,g): X → Y×Y |
| Categorical/Basic.lean | Categorical pullbacks in (2,1)-categorical sense: CategoricalPullback F G as triples (a,c,F(a)≅G(c)), with universal property for functors |
| Categorical/CatCospanTransform.lean | Morphisms between categorical cospans for 2-functoriality: transformations of cospan diagrams with CatCommSq 2-commutativity |

## Subdirectories

- [x] `Categorical/` - Categorical (2-categorical) pullbacks of functors with natural isomorphisms (complete)

## Search Tags

pullback pushout pullback-cone pushout-cocone cospan span walking-cospan pasting-lemma commutative-square is-pullback is-pushout bi-cartesian monomorphism-stability isomorphism-pullback categorical-pullback 2-categorical functor-pullback natural-isomorphism limit-cone universal-property
