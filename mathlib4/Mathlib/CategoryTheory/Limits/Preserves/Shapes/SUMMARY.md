---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Preserves/Shapes
generated: 2025-12-07T12:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 14
subdirs_count: 0
---

# Shapes

## Overview

The `Shapes/` directory provides specialized preservation results for concrete limit and colimit shapes in category theory. While the parent `Preserves/` directory establishes the general theory of limit preservation, this directory proves preservation properties for specific diagram shapes including products, pullbacks, equalizers, kernels, terminal objects, biproducts, and their duals. Each file establishes equivalences between preservation of a shape and comparison maps being isomorphisms, enabling practical verification that functors preserve specific limits by checking natural isomorphisms.

## Key Files

| File | Purpose |
|------|---------|
| BinaryProducts.lean | Binary products/coproducts preservation: equivalence between `PreservesLimit (pair X Y) G` and `prodComparison G X Y` being an isomorphism, with dual for coproducts |
| Terminal.lean | Terminal and initial objects preservation: equivalence between `PreservesLimit (Functor.empty C) G` and `terminalComparison G` being an isomorphism, includes functors inducing `IsTerminal` equivalences |
| Pullbacks.lean | Pullback and pushout preservation: equivalence between `PreservesLimit (cospan f g) G` and `pullbackComparison G f g` being an isomorphism, includes symmetry lemmas and Yoneda/coyoneda characterizations |
| Equalizers.lean | Equalizer and coequalizer preservation: equivalence between `PreservesLimit (parallelPair f g) G` and `equalizerComparison f g G` being an isomorphism, automatic preservation of split (co)equalizers |
| Products.lean | General products and coproducts preservation: equivalence between `PreservesLimit (Discrete.functor f) G` and `piComparison G f` being an isomorphism for arbitrary index types |
| Kernels.lean | Kernel and cokernel preservation in categories with zero morphisms: specialized fork preservation results for `parallelPair f 0`, requires functors preserving zero morphisms |
| Biproducts.lean | Biproduct preservation in categories with zero morphisms: defines `PreservesBiproduct` typeclass for preserving bilimit bicones, establishes biproduct comparison maps and their isomorphism characterizations |
| Zero.lean | Zero object and zero morphism preservation: defines `PreservesZeroMorphisms` typeclass, proves left/right adjoints preserve zero morphisms, equivalence with zero object preservation when both categories have zero objects |
| AbelianImages.lean | Abelian image and coimage preservation: if functor preserves kernels and cokernels, it preserves abelian images, coimages, and coimage-image comparison maps |
| Images.lean | Image preservation for functors preserving span/cospan: if functor preserves span and cospan, it preserves images via strong epi-mono factorization |
| Multiequalizer.lean | Multicoequalizer preservation: defines `MultispanIndex.map`, `Multicofork.map`, establishes `IsColimit` equivalence for multispan diagrams under functor mapping |
| Over.lean | Over/Under category preservation: if `F` preserves limits of shape `WithTerminal J`, then `Over.post F` preserves limits of shape `J`; dual for Under categories and colimits |
| Preorder.lean | Well-ordered limit preservation: defines `PreservesWellOrderContinuousOfShape J G` for functors preserving colimits at limit ordinals, composition preserves well-order continuity |
| Square.lean | Pullback/pushout square preservation: functors preserving cospans (resp. spans) preserve pullback squares (resp. pushout squares), characterization via coyoneda/yoneda functors |

## Subdirectories

(No subdirectories)

## Search Tags

preserves-shapes binary-products terminal-objects pullbacks equalizers kernels biproducts zero-morphisms products coproducts pushouts coequalizers initial-objects comparison-maps shape-preservation concrete-limits abelian-images multiequalizers over-categories under-categories well-order-continuous pullback-squares pushout-squares yoneda-characterization split-equalizers strong-epi-mono-factorization
