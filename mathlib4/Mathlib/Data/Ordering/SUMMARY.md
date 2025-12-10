---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Ordering
generated: 2025-12-11T10:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 2
subdirs_count: 0
---

# Ordering

## Overview

The `Ordering/` directory provides foundational definitions and lemmas for working with the `Ordering` type (the three-valued comparison result: `lt`, `eq`, `gt`). It defines `Compares`, which lifts an `Ordering` value to the corresponding proposition (`<`, `=`, or `>`) on ordered types, and provides `cmpUsing`/`cmp` functions for constructing `Ordering` values from decidable relations. These utilities are essential for defining and working with comparison-based operations throughout mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `Ordering.Compares` (interprets ordering as proposition), `dthen` (dependent sequencing), `cmpUsing` (lift decidable relation to Ordering), `cmp` (compare using LT instance) |
| Lemmas.lean | Simp lemmas for `Ordering`: distribution of if-then-else over ordering equality tests, `dthen`/`then` equivalence, and characterization lemmas for `cmpUsing` results (`cmpUsing_eq_lt`, `cmpUsing_eq_gt`, `cmpUsing_eq_eq`) |

## Subdirectories

*(None)*

## Search Tags

ordering comparison lt eq gt compares cmpUsing cmp decidable-relation three-way-comparison
