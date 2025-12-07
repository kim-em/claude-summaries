---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Functor
generated: 2025-12-07T20:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 15
subdirs_count: 3
---

# Functor

## Overview

The `Functor/` directory provides comprehensive formalization of functor theory in category theory, encompassing both foundational definitions and advanced categorical constructions. The module establishes the core `Functor C D` structure (notation `C ⥤ D`) with identity `𝟭` and composition `⋙`, defines the category structure on functor categories where natural transformations serve as morphisms, and develops typeclasses for special functors (fully faithful, flat, conservative) alongside preservation and reflection properties for monomorphisms, epimorphisms, and isomorphisms.

Beyond basic functor theory, the directory includes sophisticated constructions for working with product categories (constant functors, currying for bifunctors and trifunctors, hom functors) and formalizes three major advanced topics via subdirectories: (1) Kan extensions as universal solutions to functor extension problems, with pointwise characterizations via (co)limits and dense functor theory; (2) derived functors via localization theory, establishing left and right derived functors as Kan extensions and proving the derived adjunction theorem; and (3) reflection of isomorphisms with connections to balanced categories. This infrastructure supports homological algebra, algebraic topology, and other areas requiring categorical machinery.

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

- [x] `Derived/` - Derived functors via localization and Kan extensions: left derived functors as right Kan extensions, right derived functors as left Kan extensions, pointwise constructions, and derived adjunction theorem showing adjoint functors induce adjoint derived functors
- [x] `KanExtension/` - Kan extensions as universal extensions of functors: left/right Kan extensions with universal properties, pointwise characterizations via (co)limits, Kan extension functors with adjunctions to precomposition, dense functors, and preservation of Kan extensions
- [x] `ReflectsIso/` - Reflection of isomorphisms by functors: `ReflectsIsomorphisms` typeclass establishing that if `F.map f` is iso then `f` is iso, with instances for fully faithful functors and connections to balanced categories via reflection of epis/monos

## Search Tags

functors category-theory fully-faithful flat-functors preservation reflection epimorphisms monomorphisms constant-functor currying hom-functor natural-transformations functor-category bifunctors trifunctors kan-extensions left-kan-extension right-kan-extension pointwise-kan-extension derived-functors left-derived right-derived localization adjunctions dense-functors reflects-isomorphisms balanced-categories
