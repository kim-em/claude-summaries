---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/ModuleCat/Sheaf
generated: 2025-12-03T00:00:00Z
git_sha: 5bfa1623542d7f245e45ac880c26cfe8f9ecc5ea
git_branch: heads/nightly-testing
status: complete
files_count: 10
subdirs_count: 0
---

# Sheaf

## Overview

The `Sheaf/` directory establishes the categorical theory of sheaves of modules over sheaves of rings on Grothendieck sites. It proves that `SheafOfModules R` is an abelian category with all limits and colimits, constructs free sheaves of modules and their generators, and develops the pullback/pushforward functors for continuous functors between sites. The directory also introduces notions of finite type and quasicoherent sheaves of modules following the Stacks Project conventions.

## Key Files

| File | Purpose |
|------|---------|
| Abelian.lean | Proves `SheafOfModules R` is an abelian category via transfer from presheaves through the sheafification adjunction; requires sheafification and locally bijective conditions on the Grothendieck topology |
| ChangeOfRings.lean | Defines the restriction of scalars functor `restrictScalars α : SheafOfModules R' ⥤ SheafOfModules R` induced by a morphism `α : R ⟶ R'` of sheaves of rings; proves that restriction induces bijections on morphisms when the ring morphism is locally surjective and the target is a sheaf |
| Colimits.lean | Constructs colimits of arbitrary shape in `SheafOfModules R` by using the corresponding colimit in presheaves of modules and applying sheafification; requires sheafification and locally bijective conditions |
| Limits.lean | Constructs all limits in `SheafOfModules R` by showing they exist in the underlying presheaf category and verifying the limit presheaf satisfies the sheaf condition; proves evaluation and forgetful functors preserve limits; establishes preservation of finite and general limits |
| Free.lean | Constructs the free sheaf of modules functor `freeFunctor : Type u ⥤ SheafOfModules R` sending a type `I` to the coproduct of `I` copies of `unit R`; provides equivalence `freeHomEquiv` between morphisms `free I ⟶ M` and families `I → M.sections` of global sections; establishes functoriality via `freeMap` |
| Generators.lean | Defines `GeneratingSections` structure for families of global sections that generate a sheaf of modules (via epimorphism from a free sheaf); introduces `LocalGeneratorsData` for coverings of the terminal object with local generators; defines `IsFiniteType` class for sheaves of modules that are locally finitely generated; references Stacks Project tag 01B4 |
| PullbackContinuous.lean | Constructs the pullback functor `pullback φ : SheafOfModules S ⥤ SheafOfModules R` as the left adjoint to pushforward, induced by a continuous functor `F : C ⥤ D` and morphism of sheaves of rings `φ : S ⟶ F.sheafPushforward R`; proves pullback is computed by applying presheaf pullback and sheafification; establishes pseudofunctorial properties (compatibility with identity and composition) |
| PullbackFree.lean | Proves that pullback functors preserve free sheaves of modules when the underlying functor `F : C ⥤ D` is final; constructs isomorphism `pullbackObjFreeIso : (pullback φ).obj (free I) ≅ free I`; establishes natural isomorphism `freeFunctorCompPullbackIso : freeFunctor ⋙ pullback φ ≅ freeFunctor` |
| PushforwardContinuous.lean | Defines the pushforward functor `pushforward φ : SheafOfModules R ⥤ SheafOfModules S` induced by a continuous functor `F : C ⥤ D` and morphism of sheaves of rings `φ : S ⟶ F.sheafPushforward R`; proves pseudofunctorial properties (compatibility with identity via `pushforwardId` and composition via `pushforwardComp`); defines the restriction functor `over M X` for restricting a sheaf of modules to the over-category |
| Quasicoherent.lean | Defines quasicoherent sheaves of modules as those locally admitting a presentation as a cokernel of a morphism between coproducts of copies of the sheaf of rings; introduces `Presentation` structure (generators plus relations), `QuasicoherentData` (local presentations over a cover), and `IsQuasicoherent` and `IsFinitePresentation` classes; follows Stacks Project tag 01BD; proves finitely presented sheaves are automatically of finite type and quasicoherent |

## Subdirectories

(none)

## Search Tags

category-theory sheaves-of-modules sheaves-of-rings grothendieck-topology abelian-categories limits colimits free-modules generators sheafification pullback-functor pushforward-functor continuous-functors restriction-of-scalars finite-type quasicoherent locally-finitely-generated presentations stacks-project algebraic-geometry
