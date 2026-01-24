---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Span
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Span

## Overview

The `Span/` directory contains the formalization of submodule span operations in mathlib4. The core definition `Submodule.span R s` constructs the smallest submodule containing a given set `s`, with notation `R ∙ v` for singleton spans. The directory splits the theory across three files: fundamental definitions and properties (including span characterizations, Galois insertion, induction principles, and principal submodules), extended theory building on those definitions (including linear map interactions, scalar tower constructions, image/preimage properties, supremum induction, and compactness results), and specialized tensor product interactions for mixed scalar contexts (span relationships with tensor products over different base rings).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core span definitions: `Submodule.span R s` as infimum of submodules containing `s`, principal submodules (`IsPrincipal`, `generator`), membership characterization (`mem_span`, `subset_span`), span equations and monotonicity, singleton span notation `R ∙ v`, induction principles (`span_induction`, `span_induction₂`, `closure_induction`), Galois insertion with coercion, span of unions/intersections, span-sup relationships, and span over ℕ/ℤ for additive structures |
| Basic.lean | Extended span theory (875 lines): linear map compatibility (`map_span`, `span_preimage_le`, `image_span_subset`), scalar tower properties (`span_le_restrictScalars`, `span_span_of_tower`, `inclusionSpan`), span equivalences for linear maps and equivalences, unit-based span equations, supremum induction principles (`iSup_induction`, `iSup_induction'`), compactness of finitely generated submodules (`finset_span_isCompactElement`, `finite_span_isCompactElement`), product submodules (`prod`, `prod_mono`, `prod_inf_prod`, `prod_sup_prod`), and finite span extraction (`mem_span_finite_of_mem_span`) |
| TensorProduct.lean | Tensor product-span interaction for mixed scalars: natural surjection `tensorToSpan : A ⊗[R] p → span A p` for `R`-algebra `A` and `R`-submodule `p` of `A`-module `M`, equivalence `tensorEquivSpan` when `A` is flat epi over `R`, dimension preservation `finrank_span_eq_finrank : finrank A (span A p) = finrank R p` for free finite `R`-modules, and specialized results for principal ideal rings with torsion-free modules |

## Subdirectories

None - this is a leaf directory.

## Search Tags

span submodule linear-algebra generator principal-submodule galois-insertion induction-principles singleton-span tensor-product scalar-tower linear-maps image-preimage compactness finite-generation supremum product-submodules dimension-theory flat-modules
