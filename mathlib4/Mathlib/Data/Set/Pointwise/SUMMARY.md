---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Set/Pointwise
generated: 2025-12-11T17:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 0
---

# Pointwise

## Overview

The `Pointwise/` directory provides lemmas about function supports under pointwise scalar actions on sets. It shows how composing a function with an inverse scalar action transforms its support: specifically, that `support (x ↦ f (c⁻¹ • x)) = c • support f`. This connects the algebraic notion of function support with the pointwise set operations defined elsewhere in mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Support.lean | Four theorems about support/mulSupport of functions composed with inverse scalar actions: `mulSupport_comp_inv_smul` and `support_comp_inv_smul` for groups, plus `mulSupport_comp_inv_smul₀` and `support_comp_inv_smul₀` for groups with zero (requiring the scalar to be nonzero) |

## Subdirectories

*(none)*

## Search Tags

pointwise support mulSupport scalar action smul group GroupWithZero function composition inverse
