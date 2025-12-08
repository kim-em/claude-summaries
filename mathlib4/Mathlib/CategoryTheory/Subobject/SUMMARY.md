---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Subobject
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 12
subdirs_count: 0
---

# Subobject

## Overview

The `Subobject/` directory formalizes the theory of subobjects in category theory, defining `Subobject X` as the quotient by isomorphisms of monomorphisms into `X`. This provides a skeletal partial order structure on subobjects, contrasting with the thin but non-skeletal preorder `MonoOver X`. The framework includes lattice operations (meets via pullbacks, joins via images and coproducts), functorial operations (pullback, map, exists functors), factorization theory, and characterizations of well-powered categories. Special subobjects (equalizers, kernels, images) are defined along with chain conditions (Noetherian and Artinian objects) and applications to specific categories (Types, StructuredArrow, presheaves).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `Subobject X` as thin skeleton of `MonoOver X`, with coercion to ambient category, inclusion arrow, pullback/map/exists functors, and order structure |
| MonoOver.lean | Category `MonoOver X` of monomorphisms into `X` as full subcategory of `Over X`, with pullback, map, and exists functors establishing the foundational preorder structure |
| Lattice.lean | Lattice structure on subobjects: `SemilatticeInf` with `OrderTop` (via pullbacks), `SemilatticeSup` (via images and coproducts), inf/sup operations on `MonoOver` and `Subobject` |
| FactorThru.lean | Factorization predicate `P.Factors f` asserting existence of morphism through subobject `P`, with `factorThru` providing explicit factorization morphisms |
| Limits.lean | Specific subobjects from limits: `equalizerSubobject`, `kernelSubobject`, `imageSubobject` with factorization characterizations and underlying object isomorphisms |
| WellPowered.lean | Well-powered categories where `Small.{w} (Subobject X)` holds for all `X`, equivalent to `MonoOver X` being essentially small, enabling `Shrink` and `equivShrink` |
| NoetherianObject.lean | Noetherian objects with ascending chain condition on subobjects (`WellFoundedGT (Subobject X)`), as object property closed under subobjects |
| ArtinianObject.lean | Artinian objects with descending chain condition on subobjects (`WellFoundedLT (Subobject X)`), as object property closed under subobjects, dual to Noetherian in abelian categories |
| Types.lean | Proof that `Type u` is well-powered via equivalence `MonoOver α ≌ Set α` yielding order isomorphism `Subobject α ≃o Set α` for types |
| Comma.lean | Subobjects in `StructuredArrow S T` computed as subtype of subobjects of underlying right object, proving structured arrow categories are well-powered when base is |
| Presheaf.lean | Subobjects presheaf `Subobject.presheaf C : Cᵒᵖ ⥤ Type` sending objects to their subobject types and morphisms to pullback functors (requires pullbacks) |
| HasCardinalLT.lean | Cardinality preservation: if `Subobject Y` has cardinality `< κ` and `f : X ⟶ Y` is mono, then `Subobject X` has cardinality `< κ` |

## Subdirectories

None.

## Search Tags

subobjects monomorphisms skeletal-category lattice-structure pullback map-functor well-powered noetherian-objects artinian-objects factorization chain-conditions order-theory categorical-logic
