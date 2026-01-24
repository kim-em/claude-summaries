---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Group
generated: 2026-01-24T18:02:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 1
---

# Group

## Overview

The `Group/` directory contains formalizations of geometric group theory, the study of finitely generated groups through their actions on geometric spaces. The primary content focuses on group growth: for a finitely generated group G = ⟨S⟩ with finite symmetric generating set S, the growth function n ↦ |S^n| measures how the group expands under repeated multiplication. Key results include: (1) infinite groups have at least linear growth—`add_one_le_card_pow` proves n + 1 ≤ |S^n| when S generates an infinite subgroup, with `pow_right_strictMono` showing strict monotonicity; and (2) multiplicative relationships between group growth, quotient growth, and normal subgroup intersections via upper and lower bounds.

## Key Files

| File | Purpose |
|------|---------|
| README.md | Overview of geometric group theory scope and current topics covered |

## Subdirectories

- [x] `Growth/` - Group growth theory: linear lower bounds on growth of infinite groups, growth relationships between groups, normal subgroups, and quotients

## Search Tags

geometric-group-theory group-growth finitely-generated-groups generating-sets growth-function symmetric-generating-set linear-growth quotient-growth normal-subgroup strict-monotone power-of-finset closure-infinite
