---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/FunctorCategory
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 4
subdirs_count: 1
---

# FunctorCategory

## Overview

The `FunctorCategory/` directory establishes that limits and colimits in functor categories `K ⥤ C` are computed pointwise when the target category `C` has the corresponding limits. The core `Basic.lean` proves that evaluation functors jointly reflect and preserve limits, constructs limits by stitching together pointwise limit cones, and shows that a functor `F : D ⥤ K ⥤ C` preserves limits if and only if it does so at each evaluation point. Additional files provide specialized instances for epimorphisms/monomorphisms in functor categories, filtered colimits, and finite limits, with import dependencies carefully managed to avoid circular references.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of pointwise limits in functor categories: evaluation functors jointly reflect/preserve limits, `combineCones` stitches pointwise limit cones together, `functorCategoryHasLimits` instance, isomorphisms between `limit F` and `F.flip ⋙ lim`, and characterization of limit preservation via evaluation |
| EpiMono.lean | Monomorphisms and epimorphisms in functor categories characterized pointwise: `NatTrans.mono_iff_mono_app` and `NatTrans.epi_iff_epi_app` show natural transformation is mono (resp. epi) iff each component is, assuming target has pullbacks (resp. pushouts) |
| Filtered.lean | Functor categories have filtered colimits and cofiltered limits when target category does: `HasFilteredColimitsOfSize` and `HasCofilteredLimitsOfSize` instances for `K ⥤ C` |
| Finite.lean | Functor categories have finite limits and colimits when target does: instances for `HasFiniteLimits`, `HasFiniteProducts`, `HasFiniteColimits`, `HasFiniteCoproducts`, plus evaluation functors preserve finite limits/colimits |

## Subdirectories

- [x] `Shapes/` - Specific limit shapes in functor categories (complete)

## Search Tags

functor-category pointwise-limits evaluation-functor limit-preservation combine-cones jointly-reflects colimits-pointwise natural-transformations epi-mono filtered-colimits finite-limits whiskering flip-functor
