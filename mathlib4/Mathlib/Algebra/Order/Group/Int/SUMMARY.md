---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Group/Int
generated: 2025-12-01T19:35:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# Int

## Overview

The `Int/` directory contains specialized results about sums of bounded finsets of integers. It provides sharp upper and lower bounds that exploit the fact that finset elements are distinct integers, yielding tighter bounds than the naive multiplication by cardinality. The core insight is that the sum of `s` distinct integers all at most `c` cannot exceed the sum of the largest `s` consecutive integers up to `c`.

## Key Files

| File | Purpose |
|------|---------|
| Sum.lean | Sharp bounds for sums of bounded finsets of integers: `sum_le_sum_Ioc` (upper bounds using `Ioc`), `sum_le_sum_range` (upper bounds using `range`), `sum_Ico_le_sum` (lower bounds using `Ico`), `sum_range_le_sum` (lower bounds using `range`) |

## Subdirectories

(No subdirectories)

## Search Tags

integer-sums finset-bounds sharp-bounds distinct-integers bounded-sums Ioc Ico range cardinality-bounds
