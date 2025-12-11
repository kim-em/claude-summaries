---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Rat/NatSqrt
generated: 2025-12-11T13:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 2
subdirs_count: 0
---

# NatSqrt

## Overview

The `NatSqrt/` directory provides rational approximations to the square root of natural numbers. It defines `Nat.ratSqrt x prec` which computes `√(x * prec²) / prec`, giving a rational lower bound for `√x` with precision controlled by `prec`. The implementation proves both pure rational bounds (the approximation squared is at most `x`, and adding `1/prec` gives something whose square exceeds `x`) and comparisons with the real square root (the approximation is at most `√x`, and `√x` lies in an interval of width `1/prec` around it).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `Nat.ratSqrt` for rational approximation of square roots; proves `ratSqrt_nonneg`, `ratSqrt_sq_le`, and `lt_ratSqrt_add_inv_prec_sq` bounds using only rational arithmetic |
| Real.lean | Compares rational approximations with real square root; proves `ratSqrt_le_realSqrt`, `realSqrt_lt_ratSqrt_add_inv_prec`, and interval membership lemmas `realSqrt_mem_Ico`/`ratSqrt_mem_Ioc` |

## Subdirectories

(none)

## Search Tags

square-root rational-approximation Nat.ratSqrt precision bounds real-sqrt interval-approximation
