---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Shapes
generated: 2025-12-07T10:19:37Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 38
subdirs_count: 4
---

# Shapes

## Overview

The `Shapes/` directory provides the comprehensive formalization of specific limit and colimit shapes in category theory, implementing the concrete instances of universal constructions that appear throughout mathematics. At its core, it defines the fundamental shapes that every working mathematician encounters: terminal and initial objects, products and coproducts (both binary and indexed), equalizers and coequalizers, pullbacks and pushouts, and biproducts (objects that are simultaneously products and coproducts). Beyond these basics, the directory extends to specialized constructions including images and factorization systems (mono factorizations, regular/strong epi/mono), categories with zero morphisms and zero objects, wide pullbacks/equalizers for arbitrary indexing, multiequalizers for parallel families of morphisms, split equalizers with explicit splitting data, and completeness properties (finite limits, countable limits).

Each shape is implemented as a specialized case of the general limit/colimit machinery from the parent directory, with convenient notation (⊞ for biproducts, ⨁ for indexed biproducts), dedicated typeclasses (HasTerminal, HasProducts, HasPullbacks, etc.), and extensive APIs for working with universal properties specific to that shape. The subdirectories extend this foundation with: normal monomorphisms and the construction of equalizers from kernels (NormalMono/), duality between all limit shapes via opposite categories enabling systematic result transfer (Opposites/), limits in preordered types and the crucial theory of transfinite compositions for constructions by transfinite induction (Preorder/), and an extensive treatment of pullbacks encompassing pasting lemmas, commutative square formulations, and 2-categorical generalization via categorical pullbacks of functors (Pullback/). Together, this directory serves as the definitive reference for concrete universal constructions in category theory, bridging abstract limit theory with the specific shapes used throughout algebra, topology, and algebraic geometry.

## Key Files

| File | Purpose |
|------|---------|
| Terminal.lean | Initial and terminal objects as limits/colimits over empty diagrams, with HasTerminal and HasInitial typeclasses |
| Products.lean | Categorical products as limits over discrete categories: Fan cones, Pi notation, HasProducts typeclass |
| BinaryProducts.lean | Binary products and coproducts via WalkingPair indexing, with prod/coprod notation, projections, and comparison morphisms |
| Equalizers.lean | Equalizers and coequalizers as limits over parallel pairs (WalkingParallelPair), Fork cones, and universal properties |
| Kernels.lean | Kernels and cokernels as equalizers with zero morphisms, kernel.ι and kernel.lift, with properties of kernel maps |
| BinaryBiproducts.lean | Binary biproducts (simultaneous product and coproduct) with split idempotents and ⊞ notation |
| Biproducts.lean | Indexed biproducts with bicone structure (π and ι morphisms satisfying orthogonality), ⨁ notation |
| FiniteProducts.lean | Finite products as a special case, with convenience lemmas |
| FiniteLimits.lean | HasFiniteLimits typeclass for categories with all limits over finite diagrams (finitely complete) |
| WidePullbacks.lean | Wide pullbacks/pushouts over WidePullbackShape (discrete category with adjoined terminal element) |
| Images.lean | Categorical images as mono factorizations with universal property, IsImage, HasImage, HasImageMaps |
| RegularMono.lean | Regular monomorphisms (equalizers of parallel pairs) and regular epimorphisms, with RegularMono/IsRegularMono |
| StrongEpi.lean | Strong epimorphisms (lift against monomorphisms) and strong monomorphisms |
| ZeroObjects.lean | Zero objects (biterminal: simultaneously initial and terminal) with HasZeroObject typeclass |
| ZeroMorphisms.lean | Categories with designated zero morphisms in each hom-space, HasZeroMorphisms typeclass |
| IsTerminal.lean | IsTerminal and IsInitial predicates for objects satisfying terminal/initial universal properties |
| KernelPair.lean | Kernel pairs as pullbacks of morphisms with themselves |
| Multiequalizer.lean | Multiple equalizers (limits of parallel families of morphisms) |
| FiniteMultiequalizer.lean | Finite multiple equalizers |
| MultiequalizerPullback.lean | Relationship between multiequalizers and pullbacks |
| WideEqualizers.lean | Wide equalizers over arbitrary families of parallel morphisms |
| Reflexive.lean | Reflexive pairs and coequalizers of reflexive pairs (always split) |
| SplitEqualizer.lean | Split equalizers (equalizers with splitting data) |
| SplitCoequalizer.lean | Split coequalizers (coequalizers with splitting data) |
| Diagonal.lean | Diagonal morphisms and their relationship to products |
| DisjointCoproduct.lean | Disjoint coproducts with non-overlapping images |
| CombinedProducts.lean | Combined products and their properties |
| PiProd.lean | Relationship between Pi types and categorical products |
| SequentialProduct.lean | Sequential products (products indexed by natural numbers) |
| Countable.lean | Countable limits and colimits |
| StrictInitial.lean | Strict initial objects (initial objects with unique morphisms from all objects) |
| ConcreteCategory.lean | Limits in concrete categories (categories with faithful forgetful functor to Type) |
| FunctorToTypes.lean | Limits of functors to Type computed as sections |
| Grothendieck.lean | Grothendieck construction and limits in Grothendieck categories |
| End.lean | Ends (limits of bifunctors from C^op × C) |
| SingleObj.lean | Limits in single-object categories (monoids as categories) |
| Equivalence.lean | Preservation of limit shapes under equivalences |
| Connected.lean | Limits over connected diagrams |

## Subdirectories

- [x] `NormalMono/` - Normal monomorphisms (kernels of other morphisms) and construction of equalizers from kernels and finite products in normal mono categories
- [x] `Opposites/` - Duality between limit shapes via opposite categories: products↔coproducts, equalizers↔coequalizers, pullbacks↔pushouts, kernels↔cokernels, with full API for op/unop conversions
- [x] `Preorder/` - Limits in preorders as meets/joins, transfinite compositions indexed by well-ordered types, well-order-continuous functors, and HasIterationOfShape for transfinite induction
- [x] `Pullback/` - Extended pullback theory: pasting lemmas, commutative square formulation (IsPullback/IsPushout), stability under monomorphisms, and 2-categorical generalization via categorical pullbacks of functors

## Search Tags

limit-shapes colimit-shapes terminal-objects initial-objects products coproducts binary-products equalizers coequalizers kernels cokernels pullbacks pushouts biproducts finite-limits wide-pullbacks images regular-mono strong-epi zero-objects zero-morphisms mono-factorization multiequalizer reflexive-pairs split-equalizers diagonal normal-monomorphism opposite-categories duality transfinite-composition well-order-continuous pasting-lemma commutative-square categorical-pullback 2-categorical
