---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Shift
generated: 2025-12-08T15:38:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 15
subdirs_count: 0
---

# Shift

## Overview

The `Shift/` directory provides the mathematical infrastructure for shift functors in category theory, which are fundamental to the theory of triangulated categories, derived categories, and homological algebra. A shift on a category `C` indexed by a monoid `A` is implemented as a monoidal functor from `A` to the endofunctor category `C ⥤ C`, with key examples being the degree shift in chain complexes. The directory includes the core typeclass `HasShift`, functors that commute with shifts (`CommShift`), shift sequences for tracking families of shifted functors, shifted morphism spaces, and various constructions for inducing shifts on quotient categories, localized categories, and opposite categories. This framework enables systematic treatment of graded structures and homological degree shifts throughout mathlib4.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `HasShift` typeclass, `ShiftMkCore` helper structure, `shiftFunctor C a`, `shiftFunctorZero`, `shiftFunctorAdd` isomorphisms with coherence properties, and `shiftEquiv` self-equivalences when shift monoid is a group |
| ShiftSequence.lean | Type class `F.ShiftSequence M` for functors with sequence of shifted versions `F.shift a : C ⥤ A` with better definitional properties than `shiftFunctor C a ⋙ F`, includes compatibility isomorphisms and tautological shift sequence |
| CommShift.lean | Functors commuting with shifts: `F.CommShift A` typeclass with isomorphisms `shiftFunctor C a ⋙ F ≅ F ⋙ shiftFunctor D a`, construction of commutation isomorphisms for identity and composition, follows Verdier's thesis definition |
| ShiftedHom.lean | Type `ShiftedHom X Y m` for morphisms `X ⟶ Y⟦m⟧` with composition, degree zero bijection with ordinary hom, additive group structure in preadditive categories, and linear structure in linear categories |
| ShiftedHomOpposite.lean | Bijections `ShiftedHom X Y n ≃ ShiftedHom (op Y) (op X) n` and `ShiftedHom X Y a' ≃ (op (Y⟦a⟧) ⟶ (op X)⟦n⟧)` when `n + a = a'` for categories with ℤ-shift, used for homological functors in pretriangulated categories |
| Adjunction.lean | Construction of `CommShift` structure on right (or left) adjoint given `CommShift` on left (or right) adjoint, compatibility conditions between adjunction unit/counit and shift commutation isomorphisms, includes equivalences |
| Induced.lean | General mechanism to induce shift on category `D` from shift on `C` via fully faithful functor `F : C ⥤ D` when shift functors lift to `D`, used for quotient and localization shifts |
| InducedShiftSequence.lean | Induced shift sequences: given isomorphism `L ⋙ F ≅ G` and shift sequence on `G`, constructs shift sequence on `F` when `(whiskeringLeft C D A).obj L` is fully faithful, for homotopy and derived category applications |
| Localization.lean | Shift on localized categories: `W.IsCompatibleWithShift A` typeclass when morphism property preserved by shift, construction of `HasShift W.Localization A` and proof that localization functor commutes with shift |
| Quotient.lean | Shift on quotient categories: `r.IsCompatibleWithShift A` when relation preserved by shift, induced `HasShift (Quotient r) A` instance, and proof that quotient functor and lifted functors commute with shift |
| Opposite.lean | Naive shift on opposite category: `OppositeShift C A` type synonym with shift functor by `n` as `(shiftFunctor C n).op`, type synonyms for functors/natural transformations/adjunctions with pulled back `CommShift` structures |
| Pullback.lean | Pullback of shift by monoid morphism: `PullbackShift C φ` for `φ : A →+ B` has shift by `A` where shift functor by `a` is `shiftFunctor C (φ a)`, with type synonyms for functors/natural transformations/adjunctions |
| Twist.lean | Twisted shifts using center elements: `TwistShiftData C A` with invertible center elements `z a b` modifying `shiftFunctorAdd` isomorphisms while preserving shift functors, creates type synonym `t.Category` with twisted shift |
| SingleFunctors.lean | Structure `SingleFunctors C D A` for families of functors `functor a : C ⥤ D` compatible with shift on `D`, includes `shiftIso n a a' h : functor a' ⋙ shiftFunctor D n ≅ functor a` when `n + a = a'`, for single-degree complex functors |
| Linear.lean | Linearity of shift functors: proves that if localization functor `L : C ⥤ D` is `R`-linear and shift functors on `C` are `R`-linear, then shift functors on localized category `D` are also `R`-linear |

## Subdirectories

(None)

## Search Tags

shift-functors graded-categories triangulated-categories derived-categories homological-algebra degree-shift monoidal-functors shift-sequences commuting-functors shifted-morphisms localization quotient-categories opposite-categories verdier
