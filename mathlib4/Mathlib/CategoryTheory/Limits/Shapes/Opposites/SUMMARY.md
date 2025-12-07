---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Shapes/Opposites
generated: 2025-12-07T10:10:15Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# Opposites

## Overview

The `Opposites/` directory implements the duality between limits and colimits via opposite categories, establishing that limits in C correspond to colimits in Cᵒᵖ and vice versa. This fundamental categorical duality allows limit-theoretic results to be automatically dualized, providing constructions showing that products in C become coproducts in Cᵒᵖ, equalizers become coequalizers, pullbacks become pushouts, filtered colimits become cofiltered limits, and kernels become cokernels. Each file provides type class instances, natural isomorphisms between op and unop versions of diagram shapes, conversion functions between cones and cocones, and equivalences between IsLimit and IsColimit predicates.

## Key Files

| File | Purpose |
|------|---------|
| Equalizers.lean | Duality between equalizers and coequalizers: parallelPairOpIso, Fork.op/unop with IsLimit ≃ IsColimit equivalences, including specialized results for kernel pairs as pullback-pushout duals |
| Filtered.lean | Duality between filtered colimits and cofiltered limits: instances proving HasFilteredColimitsOfSize Cᵒᵖ iff HasCofilteredLimitsOfSize C |
| Kernels.lean | Duality between kernels and cokernels in categories with zero morphisms: KernelFork.IsLimit.ofιOp constructs cokernels from kernels and vice versa |
| Products.lean | Duality between products and coproducts: instances for HasProductsOfShape/HasCoproductsOfShape in opposite categories, opCoproductIsoProduct/opProductIsoCoproduct isomorphisms, Fan.op/Cofan.op with detailed interaction with Sigma.desc and Pi.lift, including binary products via opProdIsoCoprod |
| Pullbacks.lean | Duality between pullbacks and pushouts: spanOp/cospanOp/opCospan/opSpan natural isomorphisms relating diagrams, PullbackCone.op/unop and PushoutCocone.op/unop conversions, IsLimit ≃ IsColimit equivalences, canonical isomorphisms pullbackIsoUnopPushout/pushoutIsoUnopPullback with compatibility lemmas for fst/snd/inl/inr projections |

## Subdirectories

(none)

## Search Tags

opposite-categories limits-colimits-duality equalizers-coequalizers products-coproducts pullbacks-pushouts filtered-colimits cofiltered-limits kernels-cokernels op-unop cone-cocone-conversion isomorphisms fork-cofork fan-cofan pullback-cone pushout-cocone
