---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/ModuleCat
generated: 2025-12-03T15:20:00Z
git_sha: 5bfa1623542d7f245e45ac880c26cfe8f9ecc5ea
git_branch: heads/nightly-testing
status: complete
files_count: 27
subdirs_count: 5
---

# ModuleCat

## Overview

The `ModuleCat/` directory provides a comprehensive categorical treatment of R-modules, establishing `ModuleCat R` as an abelian category with all limits and colimits, complete monoidal structure (including braided, symmetric, and closed monoidal structures via tensor products), and extensive infrastructure for homological algebra. Beyond the core module category, it extends the theory to presheaves and sheaves of modules over presheaves/sheaves of rings (both abelian categories with generators and sheafification functors), topological modules with compatible continuous structures, and Kähler differentials for algebraic geometry. The directory provides change-of-rings functors (restriction, extension, coextension of scalars, pullback, and pushforward) with their adjunctions, free-forgetful adjunctions, and complete homological machinery including kernels, cokernels, exact sequences, projective/injective objects, and enough injectives. Special focus is given to finitely generated and quasicoherent sheaves following Stacks Project conventions, making this directory foundational for both abstract category theory and algebraic geometry applications.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `ModuleCat R` as bundled R-modules with morphisms as linear maps; establishes category structure, concrete category instance, and foundational isomorphism/mono/epi characterizations |
| Abelian.lean | Proves `ModuleCat R` is an abelian category; shows every mono is normal (via kernel characterization) and every epi is normal (via cokernel characterization); establishes that exactness in categorical sense corresponds to `range f = ker g` |
| ChangeOfRings.lean | Defines functors for change of rings: `restrictScalars` (views S-modules as R-modules via ring homomorphism), `extendScalars` (tensor product construction S ⊗_R M), and `coextendScalars` (internal hom construction); proves adjunctions between these functors |
| Limits.lean | Constructs all limits in ModuleCat via sections submodules; proves forgetful functor preserves limits (limits are computed pointwise on underlying types) |
| Colimits.lean | Constructs all colimits in ModuleCat; proves forgetful functor preserves colimits |
| Kernels.lean | Shows categorical kernels correspond to linear algebra kernels (as submodule with subtype map); proves categorical cokernels correspond to quotient by range |
| Monoidal/Basic.lean | Defines monoidal category structure on ModuleCat using tensor product ⊗_R as monoidal product; establishes associators, unitors, and coherence |
| Adjunctions.lean | Constructs free-forgetful adjunction where free functor sends type X to free R-module X →₀ R (finitely supported functions) and forgetful functor extracts underlying type |
| Presheaf.lean | Defines `PresheafOfModules R` for a presheaf of rings R: functors assigning to each object an R-module with restriction maps compatible with ring restriction; foundational for sheaf-theoretic module theory |
| Sheaf.lean | Defines `SheafOfModules R` for sheaf of rings R as presheaf of modules satisfying sheaf condition on underlying abelian groups; provides categorical infrastructure for sheaves of modules |
| Products.lean | Constructs categorical products in ModuleCat (direct products of modules) |
| Biproducts.lean | Proves finite biproducts exist in ModuleCat (direct sums serve as both products and coproducts); establishes biproduct structure |
| EpiMono.lean | Characterizes epimorphisms as surjective linear maps and monomorphisms as injective linear maps |
| Injective.lean | Defines and studies injective objects in ModuleCat |
| Projective.lean | Defines and studies projective objects in ModuleCat |
| EnoughInjectives.lean | Proves ModuleCat has enough injectives (every module embeds into an injective module) |
| Free.lean | Studies exact sequences involving free modules; proves that in short exact sequence with free ends, the middle module is also free |
| FilteredColimits.lean | Studies behavior of filtered colimits in ModuleCat; proves properties about preservation of filtered colimits |
| Images.lean | Defines and studies categorical images in ModuleCat; relates to range of linear maps |
| Simple.lean | Defines simple modules (no non-trivial submodules) in categorical terms |
| Subobject.lean | Studies subobject lattice structure in ModuleCat; relates categorical subobjects to submodules |
| Algebra.lean | Establishes connection between ModuleCat and AlgCat for modules that are algebras |
| AB.lean | Studies AB (Abelian-type) properties of ModuleCat |
| ExteriorPower.lean | Constructs exterior power functors on ModuleCat |
| LeftResolution.lean | Defines left resolutions in ModuleCat for homological algebra |
| Pseudofunctor.lean | Studies pseudofunctorial aspects of module categories |
| Semi.lean | Defines `SemimoduleCat R` for semirings R (modules over semirings); provides similar infrastructure as ModuleCat |
| Tannaka.lean | Studies Tannaka duality for module categories |

## Subdirectories

- [x] `Differentials/` - Kähler differentials and derivations for ring morphisms; constructs universal module of differentials with universal property; extends to presheaves of commutative rings for algebraic geometry applications
- [x] `Monoidal/` - Complete monoidal infrastructure: tensor product monoidal structure with coherence axioms, symmetric braiding via tensor commutativity, and monoidal closed structure with internal hom adjunction `M ⊗ - ⊣ ihom M`
- [x] `Presheaf/` - Full presheaf theory: abelian category structure, pointwise limits/colimits, free presheaves with adjunction, change-of-rings functors (restriction, pullback, pushforward), monoidal structure, generators, sheafification functor and adjunction for converting to sheaves
- [x] `Sheaf/` - Sheaf category infrastructure: abelian structure via sheafification transfer, limits (pointwise in presheaves) and colimits (via sheafification), free sheaves and generators, pullback/pushforward functors for continuous functors, finite type and quasicoherent sheaves (Stacks Project conventions)
- [x] `Topology/` - Topological modules category `TopModuleCat R`: limits via induced topology, colimits via coinduced topology, three adjunctions (module topology, indiscrete topology, free-forgetful), homology structure despite non-abelian nature with appropriate topological kernels/cokernels

## Search Tags

category-theory modules linear-algebra abelian-categories limits colimits monoidal-categories braided-categories symmetric-monoidal monoidal-closed tensor-products internal-hom change-of-rings restriction-of-scalars extension-of-scalars coextension-of-scalars pullback pushforward adjunctions presheaves sheaves presheaves-of-modules sheaves-of-modules homological-algebra kernels cokernels exact-sequences projective-modules injective-modules free-modules enough-injectives concrete-categories topological-modules induced-topology coinduced-topology kaehler-differentials derivations grothendieck-topology sheafification generators finite-type quasicoherent locally-finitely-generated presentations stacks-project algebraic-geometry commutative-rings ring-morphisms universal-properties continuous-functors well-powered
