---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Sites
generated: 2025-12-08T15:15:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 54
subdirs_count: 7
---

# Sites

## Overview

The `Sites/` directory provides the comprehensive formalization of Grothendieck topology and sheaf theory in mathlib4, implementing the categorical framework for gluing local data into global objects. It includes the foundational concepts (sieves, presieves, coverages), Grothendieck topologies and pretopologies, the sheaf condition in multiple equivalent forms (for types and general categories), sheafification as a left exact left adjoint, and various structural properties (cartesian closed sites, monoidal sites). The directory establishes the complete infrastructure for working with sites across multiple levels of sophistication: from basic covering families through hypercovers for higher descent, from coherent and regular topologies for concrete categories to general topos-theoretic constructions, from elementary sheaf conditions to dense subsites and comparison lemmas, from basic descent theory for prestacks to full sheaf cohomology. This machinery is fundamental for algebraic geometry, topos theory, stack theory, and any area of mathematics requiring descent theory or locality principles.

## Key Files

| File | Purpose |
|------|---------|
| Sieves.lean | Theory of sieves and presieves: sets of morphisms to an object closed under composition, with complete lattice structure and Galois insertion |
| Grothendieck.lean | Grothendieck topologies as saturated collections of sieves satisfying closure axioms, with examples (dense, atomic, discrete, trivial) |
| Pretopology.lean | Grothendieck pretopologies as bases for topologies: families of morphisms with fixed codomain satisfying axioms when pullbacks exist |
| Coverage.lean | Coverages generalizing pretopologies without requiring pullbacks, with Galois insertion between coverages and Grothendieck topologies |
| Precoverage.lean | Precoverages as building blocks for coverages |
| IsSheafFor.lean | Sheaf condition for individual presieves: compatible families of elements have unique amalgamations, with multiple equivalent formulations |
| SheafOfTypes.lean | Sheaves of types on Grothendieck topologies with equivalence to presieve-based sheaf conditions and pretopology conditions |
| Sheaf.lean | Sheaves taking values in arbitrary categories: presheaf is sheaf iff all representable copresheaves are sheaves of types |
| Sheafification.lean | HasSheafify typeclass: existence of left exact left adjoint to sheaf inclusion functor (sheafification functor) |
| Plus.lean | Plus construction P⁺ for presheaves as step toward sheafification via multiequalizers |
| CompatiblePlus.lean | Compatibility conditions for the plus construction with sheaf properties |
| CompatibleSheafification.lean | Compatibility between different sheafification approaches |
| ConcreteSheafification.lean | Concrete sheafification construction for presheaves via plus-plus construction |
| LeftExact.lean | Proof that sheafification preserves finite limits (left exactness) using filtered colimits and adhesive categories |
| EqualizerSheafCondition.lean | Sheaf condition expressed as equalizer diagram (standard in Stacks project and Mac Lane-Moerdijk) |
| Limits.lean | Limits and colimits in categories of sheaves |
| Continuous.lean | Continuous functors between sites preserving covering families |
| CoverLifting.lean | Cover lifting property: when morphisms allow lifting covers from codomain to domain |
| CoverPreserving.lean | Cover preserving functors: functors that preserve covering families |
| Equivalence.lean | Equivalences of sites and induced equivalences of sheaf categories |
| Pullback.lean | Pullback of Grothendieck topologies along functors |
| Whiskering.lean | Whiskering sheaves with functors |
| Over.lean | Sites structure on over categories with induced topologies |
| Adjunction.lean | Adjunctions between sites and their effect on sheaf categories |
| GlobalSections.lean | Global sections functor from sheaves to types/objects evaluating at terminal object |
| ConstantSheaf.lean | Constant sheaf construction associating sheaf to a fixed object |
| SheafHom.lean | Morphisms between sheaves as natural transformations |
| Subsheaf.lean | Subsheaves as monomorphisms into sheaves |
| Preserves.lean | Preservation of sheaf properties under functors |
| PreservesLocallyBijective.lean | Functors preserving locally bijective morphisms |
| PreservesSheafification.lean | Preservation of sheafification by functors |
| Localization.lean | Localization of categories with respect to Grothendieck topologies |
| EffectiveEpimorphic.lean | Effective epimorphic families and their relation to covering families |
| JointlySurjective.lean | Jointly surjective families of morphisms in sites |
| LocallyBijective.lean | Locally bijective morphisms with respect to a topology |
| LocallyFullyFaithful.lean | Locally fully faithful functors respecting site structure |
| LocallyInjective.lean | Locally injective morphisms in the context of sites |
| LocallySurjective.lean | Locally surjective morphisms and their characterization |
| EpiMono.lean | Epimorphisms and monomorphisms in categories of sheaves |
| Types.lean | Sheaves of types with additional properties and constructions |
| Spaces.lean | Grothendieck topology induced by topological spaces |
| Subcanonical.lean | Subcanonical topologies where representable presheaves are sheaves |
| CoversTop.lean | Covering families that cover the terminal object |
| Canonical.lean | Canonical topology (finest subcanonical topology) on a category |
| Finite.lean | Finite covering families and finite sites |
| Monoidal.lean | Monoidal structure on categories of sheaves |
| CartesianMonoidal.lean | Cartesian monoidal structure on sheaf categories |
| CartesianClosed.lean | Cartesian closed structure on sheaf categories |
| Closed.lean | Closed monoidal structure for sheaf categories |
| ChosenFiniteProducts.lean | Deprecated module redirecting to monoidal Cartesian modules |
| Abelian.lean | Abelian structure on categories of sheaves |
| MayerVietorisSquare.lean | Mayer-Vietoris squares for computing sheaf cohomology |
| MorphismProperty.lean | Properties of morphisms in the context of sites |
| PseudofunctorSheafOver.lean | Sheaves valued in bicategories (pseudofunctorial approach) |

## Subdirectories

- [x] `Coherent/` - Coherent, regular, and extensive Grothendieck topologies: precoherent/preregular/finitary-extensive classes with covering sieve characterizations, sheaf conditions via equalizer diagrams or finite product preservation, equivalences between sheaf categories under fully faithful functors, locally surjective/bijective properties, and relationships between the three topologies (extensive ⊔ regular generates coherent)
- [x] `DenseSubsite/` - Dense subsites and comparison lemma: cover-dense locally fully faithful functors induce equivalences of sheaf categories, allowing sheaf theory on large sites to be studied via smaller, denser subsites; includes induced topologies and sheafification compatibility
- [x] `Descent/` - Descent theory for pseudofunctors: descent data (objects over families with compatibility isomorphisms over pullbacks) and prestack condition (descent of morphisms, requiring presheaves of Hom sets are sheaves); foundational for stack theory
- [x] `Hypercover/` - Hypercovers and higher descent: 0-hypercovers (covering families with explicit indexing), 1-hypercovers (with pairwise intersection data and multifork sheaf conditions), homotopy equivalences of refinements, sheaf characterizations via hypercover families, and precoverage presentations via hypercover predicates
- [x] `NonabelianCohomology/` - Nonabelian cohomology in degree 1 for presheaves of groups: 1-cochains, 1-cocycles, cohomology relations, and quotient type H^1; extends beyond abelian Čech cohomology to non-abelian groups in low degrees
- [x] `Point/` - Points of Grothendieck sites as geometric morphisms from sets: fiber functors with cofiltered categories of elements, exactness properties, preservation of limits/colimits, and inversion of locally bijective morphisms; follows SGA 4 IV 6.3 definition
- [x] `SheafCohomology/` - Sheaf cohomology via derived functors: cohomology groups H^n as Ext-groups from constant ℤ-sheaf to abelian sheaves, and cohomology presheaves computing local cohomology at each object

## Search Tags

grothendieck-topology sites sheaves sieves coverages pretopologies sheafification descent gluing-conditions equalizer-condition plus-construction left-exact topos-theory algebraic-geometry covering-families amalgamation compatible-families yoneda-condition subcanonical representable locally-bijective coherent-topology hypercovers sheaf-cohomology
