---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring/Pointwise
generated: 2025-12-01T20:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Pointwise

## Overview

The `Pointwise/` directory provides pointwise operations on sets and finite sets in rings. It establishes that while `Set α` and `Finset α` are not themselves distributive structures (due to cross terms), pointwise operations on sets do satisfy one-sided distributivity laws. The key insight is that `s * (t + u) ⊆ s * t + s * u` (left distributivity) and `(s + t) * u ⊆ s * u + t * u` (right distributivity), though equality fails because pointwise multiplication and addition create cross terms. These files also define distributive negation instances for both sets and finite sets.

## Key Files

| File | Purpose |
|------|---------|
| Set.lean | Pointwise operations for `Set α`: distributive negation instance, subset-based left/right distributivity laws for multiplication over addition |
| Finset.lean | Pointwise operations for `Finset α`: distributive negation instance (requires `DecidableEq`), subset-based distributivity laws mirroring the set case with explicit counterexample |

## Subdirectories

(none)

## Search Tags

pointwise set-operations finset-operations distributive-negation pointwise-multiplication pointwise-addition ring-sets distributivity-subset cross-terms image2
