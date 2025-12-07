---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Constructions/Over
generated: 2025-12-07T10:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Over

## Overview

The `Over/` subdirectory provides comprehensive results on limits and colimits in over categories (slice categories). It shows how limits in `Over B` can be constructed from limits in the base category `C`: connected limits are created and preserved by the forgetful functor, products correspond to wide pullbacks, and general finite/arbitrary limits exist when the base category has appropriate pullbacks. The directory also includes dual results for under categories (coslice categories) with pushouts and coproducts.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Main module file that re-exports all over category limit constructions and declares instances for pullbacks, equalizers, finite limits (from finite wide pullbacks), and arbitrary limits (from wide pullbacks) in `Over B` |
| Connected.lean | Connected limits in over and under categories: the forgetful functor `Over B → C` creates and preserves any connected limit (limits from connected index categories), including specific constructions for cofiltered limits via `conePost` functor |
| Products.lean | Products in over categories from wide pullbacks: establishes equivalences between pullback cones and binary fans, between wide pullback diagrams and product diagrams, showing that `J`-indexed products in `Over B` correspond to `J`-indexed wide pullbacks in `C`, with dual results for pushouts and coproducts in under categories |

## Subdirectories

(none)

## Search Tags

over-category slice-category limits-in-over-category connected-limits forgetful-functor-creates-limits products-from-wide-pullbacks pullback-cone-equivalence binary-products-from-pullbacks costructured-arrow under-category coslice-category pushouts-coproducts finite-limits-over-category wide-pullbacks cofiltered-limits
