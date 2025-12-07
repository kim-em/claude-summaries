---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Constructions
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 10
subdirs_count: 1
---

# Constructions

## Overview

The `Constructions/` directory provides foundational results on constructing limits and colimits from simpler primitive limits. It shows how complex limit constructions can be built from basic building blocks: products can be constructed from pullbacks and terminal objects, equalizers from pullbacks and products, pullbacks from products and equalizers, and finite products from binary products. The directory also includes constructions for filtered/cofiltered colimits, relationships between epimorphisms/monomorphisms and limits, eventually constant functors, and special cases involving zero objects. These construction theorems are essential for establishing completeness and cocompleteness of categories by reducing the requirements to verifying a small set of primitive limits exist. The `Over/` subdirectory extends these results to over categories (slice categories), showing how limits in `Over B` can be constructed from corresponding limits in the base category, with products corresponding to wide pullbacks and connected limits being created and preserved by the forgetful functor.

## Key Files

| File | Purpose |
|------|---------|
| BinaryProducts.lean | Construct binary products from pullbacks and terminal objects; construct binary coproducts from pushouts and initial objects |
| EpiMono.lean | Relate epimorphisms and monomorphisms to limits and colimits: functors preserving/reflecting pullbacks preserve/reflect monomorphisms, and dually for pushouts and epimorphisms |
| Equalizers.lean | Construct equalizers from pullbacks and binary products; construct coequalizers from pushouts and binary coproducts, with preservation results |
| EventuallyConstant.lean | Limits and colimits of eventually constant functors from cofiltered/filtered categories, where eventually all morphisms are mapped to isomorphisms |
| Filtered.lean | Construct arbitrary colimits from finite colimits and filtered colimits; construct arbitrary limits from finite limits and cofiltered limits, including specific constructions for coproducts from finite coproducts |
| FiniteProductsOfBinaryProducts.lean | Construct finite products from binary products and terminal object; construct finite coproducts from binary coproducts and initial object, with functor preservation results |
| LimitsOfProductsAndEqualizers.lean | General theorem: construct all limits from products and equalizers; construct all finite limits from finite products and equalizers, with preservation and creation results for functors |
| Pullbacks.lean | Construct pullbacks from binary products and equalizers (pullback as equalizer of product projections); construct pushouts from binary coproducts and coequalizers |
| WeaklyInitial.lean | Construct weakly initial objects from products and weakly initial sets; construct initial objects from wide equalizers and weakly initial objects (used for General Adjoint Functor Theorem) |
| ZeroObjects.lean | Limits and colimits involving zero objects: binary products/coproducts with zero objects always exist and are isomorphic to the other factor; pullbacks/pushouts over zero objects are products/coproducts |

## Subdirectories

- [x] `Over/` - Limit constructions in over categories (slice categories) (complete)

## Search Tags

limit-constructions colimit-constructions build-limits-from-primitives products-from-pullbacks equalizers-from-products pullbacks-from-products finite-limits filtered-colimits cofiltered-limits eventually-constant-functors epi-mono-preservation zero-objects weakly-initial completeness-constructions
