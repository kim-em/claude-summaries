---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/ModuleCat
generated: 2025-12-02T12:00:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: preliminary
files_count: 27
subdirs_count: 5
---

# ModuleCat

## Overview

The `ModuleCat/` directory defines the category of R-modules (`ModuleCat R`) and establishes its rich categorical structure. It proves that ModuleCat is an abelian category with all limits and colimits, defines monoidal and symmetric structures via tensor products, and provides change-of-rings functors (restriction, extension, and coextension of scalars) with their adjunctions. The directory also extends modules to categorical contexts including presheaves and sheaves of modules over presheaves/sheaves of rings, and establishes connections to homological algebra through kernels, cokernels, exact sequences, and projective/injective objects.

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

- [x] `Differentials/` - Kähler differentials and derivations in categorical framework for modules over commutative rings (complete)
- [x] `Monoidal/` - Monoidal category structure on modules including symmetric and closed monoidal structures (complete)
- [ ] `Presheaf/` - Theory of presheaves of modules over presheaves of rings (pending)
- [ ] `Sheaf/` - Theory of sheaves of modules over sheaves of rings (pending)
- [ ] `Topology/` - Topological aspects of module categories (pending)

## Search Tags

category-theory modules linear-algebra abelian-categories limits colimits monoidal-categories tensor-products change-of-rings restriction-of-scalars extension-of-scalars adjunctions presheaves sheaves homological-algebra kernels cokernels exact-sequences projective-modules injective-modules free-modules concrete-categories
