---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Order/Group
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Group

## Overview

This directory provides measurability results for groups equipped with a lattice structure. It establishes measurability of positive and negative parts of group elements (oneLePart, leOnePart) and the multiplicative absolute value (mabs). These results are foundational for measure-theoretic analysis on ordered groups, with both multiplicative and additive versions provided through the `@[to_additive]` attribute. The file relies on the measurability infrastructure for lattice operations (MeasurableSup, MeasurableInv, MeasurableSup₂) defined elsewhere in the MeasureTheory.Order hierarchy.

## Key Files

| File | Purpose |
|------|---------|
| Lattice.lean | Measurability of group lattice operations: proves measurability of `oneLePart` (positive part, max with 1), `leOnePart` (negative part, max of inverse with 1), and `mabs` (multiplicative absolute value, supremum of element and its inverse), with both standalone theorems and compositional lemmas (Measurable.oneLePart, AEMeasurable.mabs, etc.) |

## Subdirectories

None

## Search Tags

measurable group lattice positive-part negative-part multiplicative-absolute-value oneLePart leOnePart mabs ordered-group measure-theory to-additive fun-prop
