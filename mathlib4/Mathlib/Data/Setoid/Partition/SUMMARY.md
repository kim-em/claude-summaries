---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Setoid/Partition
generated: 2025-12-11T21:45:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 0
---

# Partition

## Overview

The `Partition/` directory contains additional results about setoid partitions, specifically focused on cardinality computations. It provides a theorem showing that the cardinality of a finite set can be computed as the sum of cardinalities of its intersections with the parts of a partition.

## Key Files

| File | Purpose |
|------|---------|
| Card.lean | Provides `Setoid.IsPartition.ncard_eq_finsum`: for a partition of the ambient type and a finite set `s`, the cardinality `s.ncard` equals the `finsum` of `(s ∩ t).ncard` over all parts `t` of the partition |

## Subdirectories

None.

## Search Tags

partition cardinality ncard finsum set-intersection finite-set setoid
