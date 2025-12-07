---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Pi
generated: 2025-12-07T10:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# Pi

## Overview

The `Pi/` directory defines the pointwise category structure on indexed families of objects, enabling categories of functions from an index type `I` to objects in various categories. This provides the categorical product construction for arbitrary indexed families, generalizing binary products to dependent types. The module includes evaluation functors at each index, reindexing functors along functions between index sets, equivalences induced by index equivalences, and constructions for assembling families of functors and natural transformations into functors and natural transformations between product categories.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines category structure on `∀ i, C i` with pointwise morphisms, evaluation functors `Pi.eval`, reindexing functors `Pi.comap`, bifunctor `Pi.sum` for combining indexed families, equivalences from index type equivalences, and assembling functors/natural transformations from indexed families |

## Subdirectories

None.

## Search Tags

pi-categories product-categories indexed-families pointwise-category evaluation-functor reindexing-functor dependent-types categorical-products family-functors family-natural-transformations comap pi-eval equivalence-of-equiv option-equivalence
