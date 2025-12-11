---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Rel
generated: 2025-12-11T10:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 2
subdirs_count: 0
---

# Rel

## Overview

This folder extends the `Rel` (relations) API with notions of separation and covering for sets relative to a relation. These concepts provide quantitative tools for working with entourages in uniform spaces: `IsSeparated` captures when set elements are pairwise unrelated, while `IsCover` (aka nets) captures when a set approximates another up to the relation. Both are foundational for metric separation (`Metric.IsSeparated`) and dynamical systems (`Dynamics.IsDynNetIn`, `Dynamics.IsDynCoverOf`).

## Key Files

| File | Purpose |
|------|---------|
| Separated.lean | Defines `SetRel.IsSeparated R s` for sets whose elements are pairwise `R`-unrelated; provides lemmas for empty sets, singletons, subsingletons, monotonicity, and insertion |
| Cover.lean | Defines `SetRel.IsCover U s N` (U-covers/U-nets) where every element of `s` is `U`-close to some element of `N`; proves that maximal separated subsets are covers |

## Subdirectories

(none)

## Search Tags

relations entourage separation cover net uniform-space pairwise metric-separation dynamical-systems setrel
