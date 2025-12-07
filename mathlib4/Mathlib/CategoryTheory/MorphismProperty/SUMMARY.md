---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/MorphismProperty
generated: 2025-12-07T11:18:05Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 20
subdirs_count: 0
---

# MorphismProperty

## Overview

The `MorphismProperty/` directory provides a comprehensive framework for reasoning about classes of morphisms in category theory. It defines the fundamental type `MorphismProperty C` as predicates on morphisms, equipped with complete Boolean algebra structure, and develops an extensive API for morphism property operations including composition stability, stability under base change and cobase change, factorization systems, locality conditions, and interactions with limits and colimits. This framework is foundational for defining and working with important classes of morphisms (monomorphisms, epimorphisms, isomorphisms, relatively representable morphisms, etc.) and for applications in localization theory, model categories, site theory, and algebraic geometry.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `MorphismProperty C` as `∀ ⦃X Y : C⦄ (_ : X ⟶ Y), Prop` with complete Boolean algebra structure, opposite operations, and meta-properties `RespectsLeft`, `RespectsRight`, `Respects` |
| Composition.lean | Composition properties including type classes `ContainsIdentities`, `IsMultiplicative`, `HasTwoOutOfThreeProperty`, and predicate `IsStableUnderComposition` for morphism properties |
| Limits.lean | Stability of morphism properties under limits and colimits: `IsStableUnderBaseChange`, `IsStableUnderCobaseChange`, `universally` construction, stability under products/coproducts of various shapes |
| Representable.lean | Relatively representable morphisms with respect to functors, defining when morphisms have representable pullbacks and the `MorphismProperty.relative` construction |
| Comma.lean | Subcategories of comma categories defined by morphism properties, specializing to `P.Over Q X` for schemes étale/finite/affine over a base |
| Concrete.lean | Morphism properties in concrete categories: `injective`, `surjective`, `bijective`, with type classes `HasSurjectiveInjectiveFactorization` and functorial variants |
| Factorization.lean | Factorization axioms with structures `MapFactorizationData`, `FunctorialFactorizationData`, type classes `HasFactorization` and `HasFunctorialFactorization` for model category axioms |
| IsInvertedBy.lean | Predicate `P.IsInvertedBy F` expressing that morphisms in `P` are mapped to isomorphisms by functor `F`, used in localization theory |
| TransfiniteComposition.lean | Stability under transfinite composition of morphisms with structures `TransfiniteCompositionOfShape J` and type classes for infinite and transfinite composition stability |
| Local.lean | Locality conditions for morphism properties with respect to Grothendieck precoverages: `IsLocalAtTarget` and `IsLocalAtSource` type classes using hypercovers |
| Descent.lean | Descent theory for morphism properties including effective descent morphisms and stability properties |
| FunctorCategory.lean | Morphism properties in functor categories and their relationships to morphism properties in the target category |
| HasCardinalLT.lean | Morphism property `hasCardinalLT κ` for morphisms with small fibers (cardinality less than κ) |
| Ind.lean | Properties related to ind-objects and filtered colimits of morphisms |
| IsSmall.lean | Small morphism property for morphisms with essentially small fibers |
| LiftingProperty.lean | Lifting properties for morphisms and their interactions with other morphism properties |
| OverAdjunction.lean | Morphism properties in over categories and their behavior under adjunctions |
| Retract.lean | Retract properties expressing when morphisms are retracts of other morphisms satisfying given properties |
| RetractArgument.lean | Retract argument for showing morphism properties are stable under retracts |
| WeakFactorizationSystem.lean | Weak factorization systems as pairs of morphism properties with mutual lifting properties |

## Subdirectories

(none)

## Search Tags

morphism-property category-theory composition factorization limits base-change representable concrete-categories injective surjective localization descent transfinite-composition locality grothendieck-topology lifting-properties weak-factorization-systems model-categories
