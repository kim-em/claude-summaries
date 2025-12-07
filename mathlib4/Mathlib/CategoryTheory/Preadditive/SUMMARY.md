---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Preadditive
generated: 2025-12-07T23:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 17
subdirs_count: 3
---

# Preadditive

## Overview

The `Preadditive/` directory contains the comprehensive formalization of preadditive categories in mathlib4, which are categories where morphism sets form abelian groups and composition is bilinear. This foundational structure bridges classical category theory with homological algebra by providing the additive framework necessary for defining kernels, cokernels, exact sequences, and related constructions.

The directory is organized into three main layers: (1) **Core theory** including the definition of preadditive categories, additive functors, biproducts, Schur's lemma, matrix categories, and exactness properties; (2) **Special objects** covering injective objects (characterized by extension properties and lifting properties, with enough injectives and injective resolutions), projective objects (characterized by factorization properties and lifting properties, with enough projectives and projective resolutions), providing the infrastructure for derived functors and homological dimension theory; and (3) **Yoneda theory** specializing the Yoneda embedding to the preadditive setting with values in AddCommGrpCat and ModuleCat, characterizing injective and projective objects via epimorphism preservation.

Additional features include transfer of preadditive structure across categorical constructions (opposite categories, functor categories, algebras over additive monads/endofunctors, ind-objects), hom-orthogonal families with block diagonal decomposition, and the equivalence between additive categories and their commutative group objects.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of preadditive categories with abelian group structure on hom-sets and bilinear composition; proves mono/epi characterizations and equalizer/coequalizer constructions from kernels/cokernels |
| AdditiveFunctor.lean | Additive functors between preadditive categories that preserve the additive structure on morphisms; shows additive functors create and preserve biproducts |
| Biproducts.lean | Properties of biproducts in preadditive categories including the total formula ∑ π_j ≫ ι_j = 𝟙, Gaussian elimination for isomorphisms between biproducts, and equivalence of preserving products/coproducts/biproducts |
| Schur.lean | Schur's lemma: any nonzero morphism between simple objects in a preadditive category with kernels is an isomorphism; includes finite-dimensional version over algebraically closed fields |
| Mat.lean | Matrix category `Mat_ C` over preadditive category C with objects as finite tuples and morphisms as matrices; proves this is the additive envelope (universal property for additive functors) |
| HomOrthogonal.lean | Hom orthogonal families (distinct objects have only zero morphisms between them); block diagonal matrix decomposition for morphisms between biproducts; uniqueness of multiplicities in biproduct decompositions |
| LeftExact.lean | Left exactness of additive functors: shows that preserving kernels implies preserving all finite limits in preadditive categories; dual result for right exact functors and cokernels |
| OfBiproducts.lean | Constructs preadditive (actually semiadditive) structure from binary biproducts using Eckmann-Hilton argument to show morphisms form commutative monoids |
| Opposite.lean | Preadditive structure on opposite category Cᵒᵖ when C is preadditive; includes module structure on morphism sets |
| FunctorCategory.lean | Preadditive structure on functor categories C ⥤ D when D is preadditive, with componentwise addition |
| EilenbergMoore.lean | Preadditive structure on categories of algebras over additive monads and coalgebras over additive comonads |
| EndoFunctor.lean | Preadditive structure on algebras and coalgebras over additive endofunctors |
| Transfer.lean | Transfers preadditive structure along fully faithful functors: any fully faithful functor from C to preadditive D induces preadditive structure on C |
| SingleObj.lean | Preadditive instance for single-object category `SingleObj α` when α is a ring |
| LiftToFinset.lean | Describes legs of canonical cocones for coproducts in preadditive categories as finite sums of projections followed by inclusions |
| Indization.lean | Preadditive structure on the category of ind-objects `Ind C` when C is preadditive with finite colimits |
| CommGrp_.lean | Constructs equivalence between additive categories and their commutative group objects (additive structure maps to multiplicative structure of group objects) |

## Subdirectories

- [x] `Injective/` - Injective objects with extension properties, lifting property characterizations, enough injectives, functor preservation, and injective resolutions as cochain complexes for homological algebra
- [x] `Projective/` - Projective objects with factorization properties, internal projectivity in monoidal closed categories, lifting property characterizations, enough projectives, functor preservation, and projective resolutions as chain complexes
- [x] `Yoneda/` - Preadditive Yoneda and coyoneda embeddings lifting to AddCommGrpCat and ModuleCat with End-module structure; fully faithful additive functors preserving limits and characterizing injective/projective objects via epimorphism preservation

## Search Tags

preadditive-categories additive-functors biproducts schur-lemma matrix-categories abelian-groups hom-groups bilinear-composition additive-envelope injective-objects projective-objects eilenberg-moore algebras-over-monads left-exact right-exact kernels cokernels hom-orthogonal simple-objects
