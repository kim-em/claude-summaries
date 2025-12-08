---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/FunctorCategory
generated: 2025-12-07T21:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 1
---

# FunctorCategory

## Overview

The `FunctorCategory/` directory establishes the fundamental theory that limits and colimits in functor categories `K ⥤ C` are computed pointwise when the target category `C` has the corresponding limits. The core `Basic.lean` proves that evaluation functors jointly reflect and preserve limits, constructs limits by stitching together pointwise limit cones via `combineCones`, and characterizes limit preservation for functors into functor categories through pointwise preservation at each evaluation. Specialized files provide instances for epimorphisms/monomorphisms (characterized pointwise via components), filtered colimits and cofiltered limits, and finite limits/colimits. The `Shapes/` subdirectory demonstrates how this general pointwise theory instantiates for classical categorical constructions (products, pullbacks, kernels), providing explicit isomorphisms showing that evaluating a limit of functors yields the limit of evaluated functors.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of pointwise limits in functor categories: evaluation functors jointly reflect/preserve limits, `combineCones` stitches pointwise limit cones together, `functorCategoryHasLimits` instance, isomorphisms between `limit F` and `F.flip ⋙ lim`, and characterization of limit preservation via evaluation |
| EpiMono.lean | Monomorphisms and epimorphisms in functor categories characterized pointwise: `NatTrans.mono_iff_mono_app` and `NatTrans.epi_iff_epi_app` show natural transformation is mono (resp. epi) iff each component is, assuming target has pullbacks (resp. pushouts) |
| Filtered.lean | Functor categories have filtered colimits and cofiltered limits when target category does: `HasFilteredColimitsOfSize` and `HasCofilteredLimitsOfSize` instances for `K ⥤ C` |
| Finite.lean | Functor categories have finite limits and colimits when target does: instances for `HasFiniteLimits`, `HasFiniteProducts`, `HasFiniteColimits`, `HasFiniteCoproducts`, plus evaluation functors preserve finite limits/colimits |

## Subdirectories

- [x] `Shapes/` - Specific limit shapes in functor categories

## Search Tags

functor-category pointwise-limits evaluation-functor limit-preservation combine-cones jointly-reflects colimits-pointwise natural-transformations epi-mono filtered-colimits finite-limits whiskering flip-functor
