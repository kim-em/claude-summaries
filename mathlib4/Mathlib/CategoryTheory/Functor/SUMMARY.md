---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Functor
generated: 2025-12-07T16:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 15
subdirs_count: 3
---

# Functor

## Overview

The `Functor/` directory contains the core theory of functors between categories, including their basic properties, typeclasses for special functors (fully faithful, flat, conservative), and various constructions (constant functors, currying, hom functors). This module provides the foundational structure `Functor C D` representing functors from category `C` to category `D` with the notation `C ⥤ D`, along with the identity functor `𝟭`, composition `⋙`, and the category structure on functor categories. It includes preservation and reflection properties (monomorphisms, epimorphisms, isomorphisms), flatness characterizations, and utility functors for working with product categories and higher-order functors (bifunctors, trifunctors).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core functor definition with `obj` and `map` preserving identities and composition, identity functor `𝟭`, and composition `⋙` |
| Category.lean | Category instance on functor categories `C ⥤ D` with natural transformations as morphisms, plus left/right unitors and associator |
| FullyFaithful.lean | Typeclasses `Full` (surjective on morphisms) and `Faithful` (injective on morphisms), with `FullyFaithful` structure containing inverse `preimage` |
| EpiMono.lean | Preservation and reflection of monomorphisms and epimorphisms via typeclasses `PreservesMonomorphisms`, `PreservesEpimorphisms`, `ReflectsMonomorphisms`, `ReflectsEpimorphisms` |
| Flat.lean | Representably flat functors (comma category is cofiltered) with equivalence to preserving finite limits when domain has finite limits |
| Const.lean | Constant functor `const J : C ⥤ (J ⥤ C)` sending every object in `J` to a fixed `X : C` and every morphism to `𝟙 X` |
| Currying.lean | Curry/uncurry functors establishing equivalence `(C ⥤ (D ⥤ E)) ≌ ((C × D) ⥤ E)` for product categories |
| CurryingThree.lean | Extension of currying to three-variable functors with `(C ⥤ D ⥤ E ⥤ H) ≌ ((C × D × E) ⥤ H)` |
| Hom.lean | Hom functor `Cᵒᵖ × C ⥤ Type v` sending `(X, Y)` to morphisms `X ⟶ Y`, contravariant in first argument and covariant in second |
| FunctorHom.lean | Functor hom-sets and evaluation functors for functor categories |
| Functorial.lean | Typeclass for functorial properties of constructions |
| Trifunctor.lean | Trifunctors obtained by composing bifunctors: `bifunctorComp₁₂` and `bifunctorComp₂₃` |
| OfSequence.lean | Functors constructed from sequences of objects and morphisms |
| TwoSquare.lean | Two-square diagrams and their functorial properties |
| TypeValuedFlat.lean | Flat type-valued functors (distinct from representably flat functors) |

## Subdirectories

- [ ] `Derived/` - Derived functors (pending)
- [ ] `KanExtension/` - Kan extensions (left and right adjoints along functors) (pending)
- [ ] `ReflectsIso/` - Reflection of isomorphisms by functors (pending)

## Search Tags

functors category-theory fully-faithful flat-functors preservation reflection epimorphisms monomorphisms constant-functor currying hom-functor natural-transformations functor-category bifunctors trifunctors
