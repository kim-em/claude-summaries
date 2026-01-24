---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Group/Growth
generated: 2026-01-24T17:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Growth

## Overview

This folder contains formalizations of group growth theory within geometric group theory. For a finitely generated group G = ⟨S⟩ with finite symmetric generating set S, the growth function n ↦ |S^n| measures how the group expands under repeated multiplication. The main results establish: (1) infinite groups have at least linear growth—if S generates an infinite subgroup, then |S^n| ≥ n + 1; and (2) the growth of a group relates multiplicatively to the growth in a normal subgroup and its quotient, providing both upper and lower bounds.

## Key Files

| File | Purpose |
|------|---------|
| README.md | Overview of group growth theory and topics covered |
| LinearLowerBound.lean | Proves that sets generating infinite groups have at least linear growth: `add_one_le_card_pow` shows n + 1 ≤ |S^n|. Key intermediate results include `pow_right_strictMono` showing S^n is strictly increasing in n when the closure is infinite |
| QuotientInter.lean | Relates growth in a group to growth in quotients and intersections with normal subgroups. `card_pow_quotient_mul_pow_inter_subgroup_le` gives upper bound; `le_card_quotient_mul_sq_inter_subgroup` gives lower bound for symmetric sets |

## Subdirectories

*None*

## Search Tags

group-growth growth-function linear-growth finitely-generated-groups generating-set symmetric-generating-set quotient-group normal-subgroup geometric-group-theory strict-monotone power-of-finset closure-infinite
