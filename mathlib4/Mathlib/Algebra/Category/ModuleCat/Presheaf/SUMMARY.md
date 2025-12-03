---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/ModuleCat/Presheaf
generated: 2025-12-03T14:30:00Z
git_sha: 5bfa1623542d7f245e45ac880c26cfe8f9ecc5ea
git_branch: heads/nightly-testing
status: complete
files_count: 12
subdirs_count: 0
---

# Presheaf

## Overview

The `Presheaf/` directory develops the comprehensive theory of presheaves of modules over presheaves of rings. It establishes that the category `PresheafOfModules R` is abelian with all limits and colimits, provides change-of-rings functors (restriction of scalars, pullback, and pushforward), constructs free presheaves of modules with adjunctions, and implements monoidal category structure via pointwise tensor products. The directory also contains the sheafification machinery for converting presheaves of modules to sheaves of modules, including the construction of the associated sheaf functor and its adjunction with the forgetful functor.

## Key Files

| File | Purpose |
|------|---------|
| Abelian.lean | Proves `PresheafOfModules R` is an abelian category by showing it has normal epis (via kernel characterization) and normal monos (via cokernel characterization); imports colimits, limits, and abelian infrastructure |
| ChangeOfRings.lean | Defines restriction of scalars functor `restrictScalars α : PresheafOfModules R' ⥤ PresheafOfModules R` for morphism of presheaves of rings `α : R ⟶ R'`; shows the functor is additive and faithful |
| Colimits.lean | Constructs all colimits in `PresheafOfModules R` by computing them pointwise (taking colimits in `ModuleCat (R.obj X)` for each object X); proves evaluation and forgetful functors preserve colimits; includes finite colimits as special case |
| EpiMono.lean | Characterizes epimorphisms as pointwise surjective morphisms and monomorphisms as pointwise injective morphisms; provides `epi_iff_surjective` and `mono_iff_injective` characterizations |
| Free.lean | Constructs free presheaf of modules functor `free R : (Cᵒᵖ ⥤ Type u) ⥤ PresheafOfModules R` that sends presheaf of types to presheaf of free modules; establishes `freeAdjunction` showing this is left adjoint to forgetful functor |
| Generator.lean | Studies generating objects in `PresheafOfModules R`; defines `freeYoneda R` (free presheaves on Yoneda representables) and proves they form a separating and detecting set; shows presheaves of modules are well-powered; constructs canonical presentations via coproducts of free Yoneda objects |
| Limits.lean | Constructs all limits in `PresheafOfModules R` by computing them pointwise (taking limits in `ModuleCat (R.obj X)` for each object X); proves evaluation and forgetful functors preserve limits; includes finite limits as special case |
| Monoidal.lean | Defines monoidal category structure on `PresheafOfModules (R ⋙ forget₂ _ _)` for commutative ring presheaf R; tensor product defined pointwise `(M₁ ⊗ M₂).obj X = M₁.obj X ⊗ M₂.obj X`; establishes associators, unitors, and all monoidal coherence axioms |
| Pullback.lean | Constructs pullback functor `pullback φ : PresheafOfModules S ⥤ PresheafOfModules R` as left adjoint to pushforward for morphism `φ : S ⟶ F.op ⋙ R`; proves existence under universe assumptions; establishes pullback composition isomorphisms and pseudofunctor-like properties |
| Pushforward.lean | Constructs pushforward functor `pushforward φ : PresheafOfModules R ⥤ PresheafOfModules S` induced by morphism of presheaves of rings `φ : S ⟶ F.op ⋙ R` where `F : C ⥤ D`; shows compatibility with composition and identity (pseudofunctor properties) |
| Sheafification.lean | Constructs sheafification functor `sheafification α : PresheafOfModules R₀ ⥤ SheafOfModules R` for locally bijective morphism `α : R₀ ⟶ R.val`; establishes adjunction `sheafification α ⊣ SheafOfModules.forget R ⋙ restrictScalars α`; proves sheafification preserves finite limits |
| Sheafify.lean | Low-level construction of associated sheaf for presheaf of modules; given sheafification maps `α : R₀ ⟶ R.val` and `φ : M₀.presheaf ⟶ A.val`, defines scalar multiplication on sheafified abelian group using compatible families; constructs `sheafify α φ : SheafOfModules R` with canonical map `toSheafify : M₀ ⟶ restrictScalars α (sheafify α φ)` |

## Subdirectories

None.

## Search Tags

category-theory presheaves-of-modules abelian-categories limits colimits change-of-rings restriction-of-scalars pullback pushforward free-modules adjunctions generators monoidal-categories tensor-products sheafification associated-sheaf Grothendieck-topology locally-bijective epimorphisms monomorphisms well-powered presheaves-of-rings
