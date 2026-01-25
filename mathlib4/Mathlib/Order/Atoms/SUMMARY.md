---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Atoms
generated: 2026-01-25T19:35:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 1
subdirs_count: 0
---

# Atoms

## Overview

The `Atoms/` subdirectory contains specialized results about atoms and coatoms in finite and locally finite contexts. This complements the main `Order/Atoms.lean` file by providing finiteness-specific theorems, including that finite partial orders with boundaries are automatically atomic/coatomic, and establishing the relationship between simple orders and Boolean finiteness.

## Key Files

| File | Purpose |
|------|---------|
| Finite.lean | Atoms/coatoms in finite and locally finite orders: proves finite partial orders with bottom are atomic (Finite.to_isAtomic) and with top are coatomic (Finite.to_isCoatomic); establishes IsSimpleOrder implies Fintype with cardinality 2; proves locally finite orders are strongly atomic/coatomic; includes results on infinite sets with finite covering relations |

## Subdirectories

*(No subdirectories)*

## Search Tags

atoms coatoms finite-order locally-finite simple-order atomic coatomic strongly-atomic fintype covering-relation
