---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category
generated: 2025-12-04T12:00:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 3
subdirs_count: 13
---

# Category

## Overview

The `Category/` directory provides a comprehensive categorical treatment of algebraic structures in mathlib4, implementing bundled categories where algebraic objects (groups, monoids, rings, modules, algebras, bialgebras, coalgebras, Hopf algebras) become category-theoretic objects with structure-preserving morphisms. The directory establishes the complete categorical infrastructure for each algebraic structure, including forgetful functors between related categories, all limits and colimits, adjunctions (free-forgetful, abelianization, change of rings), monoidal structures using tensor products, and categorical equivalences (ℤ-modules ≃ abelian groups, algebras as objects under commutative rings, coalgebras ≃ comonoid objects in modules). Major results include proving `AddCommGrpCat` and `ModuleCat` are abelian categories satisfying Grothendieck's AB axioms, establishing essential smallness of finitely generated categories, providing enough injectives/projectives, and developing specialized theories for presheaves/sheaves of modules, topological modules, continuous cohomology, and Kähler differentials for algebraic geometry applications.

## Key Files

| File | Purpose |
|------|---------|
| BoolRing.lean | Category of Boolean rings with morphisms as ring homomorphisms; defines forgetful functor to `CommRingCat` and equivalence with `BoolAlg` (Boolean algebras as categories) |
| CommBialgCat.lean | Category of commutative bialgebras over a commutative ring `R` with morphisms as bialgebra homomorphisms; includes forgetful functor to `CommAlgCat` and equivalence with comonoid objects in `(CommAlgCat R)ᵒᵖ` |
| GrpWithZero.lean | Category of groups with zero (`GroupWithZero`) with morphisms as monoid-with-zero homomorphisms; includes forgetful functors to `MonCat` and `Bipointed` |

## Subdirectories

- [x] `AlgCat/` - Category of algebras over commutative rings with complete infrastructure: forgetful functors to rings/modules, free algebra construction with adjunction, all limits with preservation, and symmetric monoidal structure via tensor products
- [x] `AlgebraCat/` - Deprecated re-exports providing backward compatibility for symmetric monoidal structure (moved to AlgCat.Monoidal and ModuleCat.Monoidal.Symmetric as of May 2025)
- [x] `BialgCat/` - Category of bialgebras combining algebra and coalgebra structures: forgetful functors to both AlgCat and CoalgCat, monoidal structure with tensor products making both forgetful functors monoidal
- [x] `CoalgCat/` - Category of coalgebras with monoidal structure via tensor products, equivalence with comonoid objects in ModuleCat, and compatibility proofs for comultiplication/counit on tensor products
- [x] `CommAlgCat/` - Category of commutative algebras: equivalence with rings under R (Under R), braided monoidal structure with tensor products, Cartesian structure on opposite category, and finitely generated subcategory (FGAlgCat) proven essentially small
- [x] `ContinuousCohomology/` - Continuous cohomology for topological groups acting on topological modules: homology functor from Action(TopModuleCat R)G to cochain complexes using inductive homogeneous cochains C(G,C(G,...,M)) with H⁰≅invariants
- [x] `FGModuleCat/` - Category of finitely generated modules: monoidal structure (commutative rings), closed monoidal and right-rigid with duality (fields), abelian category (Noetherian rings), finite limits/colimits, and essential smallness via explicit quotient representations
- [x] `Grp/` - Comprehensive group category theory: GrpCat/AddGrpCat/CommGrpCat/AddCommGrpCat with all limits/colimits, AddCommGrpCat as abelian category satisfying Grothendieck AB axioms (AB4, AB4*, AB5), ℤ-module equivalence, free-forgetful adjunctions, abelianization, injective objects via divisibility/character modules, finite group subcategories, and Cartesian monoidal structure
- [x] `HopfAlgCat/` - Category of Hopf algebras with morphisms as bialgebra homomorphisms: forgetful functor to BialgCat (monoidal), tensor product monoidal structure, and iso/BialgEquiv conversions
- [x] `ModuleCat/` - Extensive module category infrastructure: abelian category with all limits/colimits, symmetric closed monoidal structure via tensor/internal hom, change-of-rings functors with adjunctions (restrict/extend/coextend scalars, pullback/pushforward), presheaves/sheaves of modules as abelian categories with sheafification and generators, topological modules with three adjunctions, Kähler differentials for algebraic geometry, free-forgetful adjunction, homological algebra (kernels/cokernels/exact sequences/projective/injective/enough injectives), and finitely generated/quasicoherent sheaves following Stacks Project
- [x] `MonCat/` - Category of monoids and commutative monoids: MonCat/AddMonCat/CommMonCat/AddCommMonCat with all limits/colimits, filtered colimits preservation, free-forgetful and adjoin-one adjunctions, corepresentability of forgetful functors (by ULift ℕ), and CommMonCat-valued Yoneda embeddings
- [x] `Ring/` - Ring category infrastructure: SemiRingCat/RingCat/CommSemiRingCat/CommRingCat with all limits/colimits, filtered colimits preservation, free-forgetful adjunctions (ℤ[X] for commutative rings), tensor products as pushouts/coproducts, epimorphism characterization (surjective ⇔ epi+finite), finitely presented rings, topology on Hom(A,R) for topological rings, and Under R subcategory for R-algebras with base change functors
- [x] `Semigrp/` - Bundled categories for magmas and semigroups: MagmaCat/AddMagmaCat/Semigrp/AddSemigrp with concrete category instances, morphisms as homomorphisms, forgetful functors, and MulEquiv/isomorphism conversions

## Search Tags

category-theory algebra categorical-algebra bundled-categories groups rings modules algebras bialgebras coalgebras hopf-algebras boolean-rings forgetful-functors categorical-equivalences monads concrete-categories morphisms abelian-categories limits colimits monoidal-categories symmetric-monoidal braided-monoidal closed-monoidal adjunctions free-forgetful grothendieck-axioms AB4 AB5 tensor-products internal-hom homological-algebra kernels cokernels exact-sequences projective-objects injective-objects enough-injectives presheaves sheaves sheafification topological-modules kaehler-differentials change-of-rings restriction-scalars extension-scalars coextension-scalars pullback pushforward finite-presentation essential-smallness duality rigid-categories continuous-cohomology comonoid-objects quasicoherent-sheaves algebraic-geometry
