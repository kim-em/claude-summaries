---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Shapes
generated: 2025-12-07T12:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 38
subdirs_count: 4
---

# Shapes

## Overview

The `Shapes/` directory provides the formalization of specific limit and colimit shapes in category theory, implementing the concrete instances of universal constructions that appear throughout mathematics. It includes basic shapes (terminal/initial objects, binary/indexed products and coproducts), equalizers and coequalizers (including kernels and cokernels in categories with zero morphisms), pullbacks and pushouts (including wide variants), biproducts (simultaneous products and coproducts), images and factorization systems (mono factorizations, regular/strong epi/mono), and special properties (finite limits, countable limits, reflexive pairs, strict initial objects, zero objects/morphisms). Each shape is implemented as a specialized case of the general limit/colimit machinery, with convenient abbreviations and lemmas for working with the universal properties specific to that shape.

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

- [x] `NormalMono/` - Normal monomorphisms and related theory (complete)
- [x] `Opposites/` - Duality between limit shapes via opposite categories (complete)
- [x] `Preorder/` - Limits in preorders as meets/joins, transfinite compositions (complete)
- [x] `Pullback/` - Extended theory of pullbacks including pasting lemmas, monoicity, commutative squares, and 2-categorical perspectives (complete)

## Search Tags

limit-shapes colimit-shapes terminal-objects initial-objects products coproducts binary-products equalizers coequalizers kernels cokernels pullbacks pushouts biproducts finite-limits wide-pullbacks images regular-mono strong-epi zero-objects zero-morphisms mono-factorization multiequalizer reflexive-pairs split-equalizers diagonal
