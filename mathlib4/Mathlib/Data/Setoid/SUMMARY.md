---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Setoid
generated: 2025-12-11T21:50:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 2
subdirs_count: 1
---

# Setoid

## Overview

The `Setoid/` directory provides the mathematical infrastructure for setoids (types equipped with equivalence relations) and their associated partitions. It defines the complete lattice structure on equivalence relations, the correspondence between equivalence relations and partitions, and various isomorphism theorems for quotients. The `Partition/` subdirectory extends this with cardinality computations for finite sets intersected with partition parts. Together, this forms a foundational component for reasoning about quotient types and equivalence classes throughout mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Complete lattice of equivalence relations on a type; kernel of functions as setoids; equivalence closure; product/pi setoids; isomorphism theorems (first, second, third) for quotients; Galois insertion between relations and setoids; correspondence between setoids containing r and setoids on Quotient r |
| Partition.lean | Partitions as set collections (`IsPartition`); equivalence between partitions and setoids (`Partition.orderIso`); `IndexedPartition` structure for indexed families with constructive access (index, some, proj, out); complete lattice on partitions; conversion to/from `Finpartition`; piecewise function construction from partitions |

## Subdirectories

- [x] `Partition/` - Additional results about partitions (cardinality computations)

## Search Tags

setoid equivalence-relation partition quotient equivalence-class kernel complete-lattice isomorphism-theorems indexed-partition pairwise-disjoint
