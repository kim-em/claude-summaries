---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/GroupWithZero/Pointwise
generated: 2025-12-01T18:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 1
subdirs_count: 1
---

# Pointwise

## Overview

The `Pointwise/` directory provides the complete theory of pointwise operations on both infinite sets and finite sets in the context of groups with zero. This extends the general pointwise operation theory to handle zero-specific phenomena: how multiplication and division by zero collapse to trivial sets (for nonempty inputs), how nonzero scalars preserve set cardinality via injectivity, and how cancellation properties yield cardinality inequalities for finite sets. The `Set/` subdirectory handles infinite set theory using cardinals, while `Finset.lean` provides the corresponding finite set results using natural number cardinalities.

## Key Files

| File | Purpose |
|------|---------|
| Finset.lean | Pointwise operations on finite sets in groups with zero: cardinality inequalities for multiplication (card_le_card_mul_left₀, card_le_card_mul_right₀) using cancellation properties, zero multiplication/division behavior (s * 0 = 0, s / 0 = 0 for nonempty s), and inverse of singleton zero |

## Subdirectories

- [x] `Set/` - Pointwise operations on infinite sets: zero multiplication/division collapsing behavior, cardinality preservation for nonzero scalar multiplication via Cardinal.mk_smul_set₀ and natCard_smul_set₀ (complete)

## Search Tags

pointwise-operations set-multiplication finset-multiplication group-with-zero zero-behavior cardinality-bounds cancellation division-by-zero scalar-multiplication
