---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Final
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Final

## Overview

The `Final/` directory contains specialized results about final and initial functors, building on the core theory in `Final.lean` at the parent level. It establishes characterizations of connected categories via constant functors to discrete categories, conditions under which parallel pair diagrams are initial, and explicit constructions showing that initial/final functors induce bijections on sections and colimit types of functors to Type. These results are crucial for understanding when limits can be computed along certain functors and for working with colimits in categories of types.

## Key Files

| File | Purpose |
|------|---------|
| Connected.lean | Connected categories characterized as categories where constant functor to discrete singleton is final/initial; proves product projections are final/initial when other factor is connected |
| ParallelPair.lean | Sufficient conditions for parallel pair diagrams to be initial: existence of morphisms from source and factorization of parallel morphisms through the pair |
| Type.lean | Action of initial/final functors on sections and colimit types: `sectionsPrecomp` is bijective for initial functors, `colimitTypePrecomp` is bijective for final functors |

## Subdirectories

(none)

## Search Tags

final-functors initial-functors connected-categories parallel-pairs costructured-arrow structured-arrow sections colimit-type functors-to-types bijection categorical-connectivity zigzag
