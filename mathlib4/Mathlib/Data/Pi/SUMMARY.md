---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Pi
generated: 2025-12-11T10:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 0
---

# Pi

## Overview

The `Pi/` directory contains infrastructure for working with dependent function types (Π-types) in the context of finite ordered structures. Currently it provides a single file that establishes locally finite order instances for pi types, allowing interval operations and cardinality calculations on dependent functions to locally finite orders.

## Key Files

| File | Purpose |
|------|---------|
| Interval.lean | Establishes that dependent functions to locally finite orders are themselves locally finite; provides `LocallyFiniteOrder`, `LocallyFiniteOrderBot`, and `LocallyFiniteOrderTop` instances for pi types; includes cardinality formulas for intervals `Icc`, `Ico`, `Ioc`, `Ioo`, `Iic`, `Iio`, `Ici`, `Ioi`, and `uIcc` as products over components |

## Subdirectories

None.

## Search Tags

pi-types dependent-functions locally-finite-order intervals cardinality piFinset pointwise-order fintype
