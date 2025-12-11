---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Set/Card
generated: 2025-12-11T20:45:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 0
---

# Card

## Overview

The `Card/` directory contains results about set cardinality that require cardinal arithmetic imports. This is separated from the main `Data/Set/Card.lean` file to avoid burdening it with extra imports from `SetTheory.Cardinal.Arithmetic`. The file provides theorems about splitting sets with even cardinality into equal-sized disjoint halves, and lemmas for computing cardinalities of unions.

## Key Files

| File | Purpose |
|------|---------|
| Arithmetic.lean | Cardinal arithmetic results for sets: splitting even-cardinality sets into equal disjoint halves, cardinality of indexed unions (`biUnion`, `iUnion`) with `ncard` and `encard`, upper bounds for union cardinalities, and `finsum_one` lemma |

## Subdirectories

(none)

## Search Tags

set cardinality ncard encard cardinal arithmetic even disjoint union biUnion iUnion finsum pairwise-disjoint
