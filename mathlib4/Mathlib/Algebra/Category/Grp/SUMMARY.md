---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/Grp
generated: 2025-12-02T00:00:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 27
subdirs_count: 0
---

# Grp

## Overview

The `Grp/` directory provides the categorical infrastructure for groups and abelian groups in Lean's mathlib4. It defines bundled categories `GrpCat`, `AddGrpCat`, `CommGrpCat`, and `AddCommGrpCat` along with their morphisms, forgetful functors, and categorical properties. The directory establishes that these categories have all limits and colimits, proves that `AddCommGrpCat` is an abelian category satisfying Grothendieck's AB axioms, demonstrates equivalences (including the fundamental equivalence between ℤ-modules and abelian groups), and provides adjunctions, injectivity results, and specialized subcategories like finite groups.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `GrpCat`, `AddGrpCat`, `CommGrpCat`, `AddCommGrpCat` with bundled category instances; defines morphisms as group homomorphisms and concrete category structure |
| Limits.lean | Proves that the category of groups has all limits, constructed as subgroups of sections; shows forgetful functors preserve limits |
| Colimits.lean | Constructs all colimits in `AddCommGrpCat` as quotients of direct sums (finitely supported functions) modulo diagram relations |
| Preadditive.lean | Establishes that `AddCommGrpCat` is a preadditive category with morphism addition, negation, and abelian group structure on hom-sets |
| Abelian.lean | Proves that `AddCommGrpCat` is an abelian category by showing every mono/epi is normal, using the equivalence with ℤ-modules |
| AB.lean | Proves `AddCommGrpCat` satisfies Grothendieck's axioms AB5 (filtered colimits preserve finite limits), AB4, and AB4* |
| ZModuleEquivalence.lean | Establishes the categorical equivalence between ℤ-modules and abelian groups via the forgetful functor `forget₂ (ModuleCat ℤ) AddCommGrpCat` |
| Biproducts.lean | Shows `AddCommGrpCat` has finite biproducts and verifies they coincide with categorical products/coproducts via Cartesian products |
| Kernels.lean | Proves that concrete kernels (as subgroups) and cokernels (as quotients) are categorical kernels and cokernels in `AddCommGrpCat` |
| Adjunctions.lean | Constructs free group and free abelian group functors; proves adjunctions between free functors and forgetful functors; defines abelianization functor |
| EquivalenceGroupAddGroup.lean | Provides equivalences between multiplicative and additive versions: `GrpCat ≌ AddGrpCat` and `CommGrpCat ≌ AddCommGrpCat` via `Additive`/`Multiplicative` |
| FilteredColimits.lean | Proves that forgetful functors from group categories preserve filtered colimits by showing filtered colimits carry group structure |
| Injective.lean | Proves divisible abelian groups are injective objects using Baer's criterion for ℤ-modules |
| EnoughInjectives.lean | Establishes that `AddCommGrpCat` and `CommGrpCat` have enough injectives via character module embeddings into products of ℚ/ℤ |
| EpiMono.lean | Characterizes epimorphisms and monomorphisms in group categories (typically as surjective and injective homomorphisms) |
| FiniteGrp.lean | Defines `FiniteGrp` and `FiniteAddGrp` categories of finite groups with induced category structure from `GrpCat` |
| Images.lean | Constructs categorical images in group categories, showing they correspond to homomorphic images (range subgroups) |
| Subobject.lean | Relates categorical subobjects in `AddCommGrpCat` to actual subgroups |
| Zero.lean | Establishes that group categories have zero objects (the trivial group) |
| ForgetCorepresentable.lean | Shows forgetful functors are corepresentable by appropriate groups (e.g., ℤ for abelian groups) |
| CartesianMonoidal.lean | Proves group categories have Cartesian monoidal structure with products as tensor |
| ChosenFiniteProducts.lean | Provides explicit chosen finite products for computational purposes |
| LargeColimits.lean | Extends colimit constructions to large diagram shapes |
| LeftExactFunctor.lean | Studies left exact functors from group categories (functors preserving finite limits) |
| IsFinite.lean | Properties and results about finite groups within the categorical framework |
| Yoneda.lean | Applications of the Yoneda lemma to group categories |
| Ulift.lean | Relates groups in different universes via `ULift` universe-lifting functor |

## Subdirectories

*(none)*

## Search Tags

category-theory groups abelian-groups bundled-categories limits colimits abelian-category grothendieck-axioms AB5 AB4 preadditive biproducts kernels cokernels injective-objects free-groups abelianization adjunctions equivalences filtered-colimits finite-groups additive multiplicative concrete-category forgetful-functors monomorphisms epimorphisms
