---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/FreeAbelianGroup
generated: 2025-12-01T15:42:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# FreeAbelianGroup

## Overview

This directory establishes the canonical isomorphism between `FreeAbelianGroup X` and finitely supported functions `X →₀ ℤ`, providing a concrete representation of free abelian groups. The isomorphism enables the transport of support-related notions from `Finsupp` to `FreeAbelianGroup`, including coefficient extraction and support computation. Additionally, it proves that free abelian groups satisfy the `TwoUniqueSums` property, which ensures uniqueness of representation in sums.

## Key Files

| File | Purpose |
|------|---------|
| Finsupp.lean | Constructs the group isomorphism `FreeAbelianGroup.equivFinsupp : FreeAbelianGroup X ≃+ (X →₀ ℤ)` and uses it to define `coeff` (multiplicity of an element) and `support` (finite set of occurring elements) with their basic properties |
| UniqueSums.lean | Proves the `TwoUniqueSums` instance for `FreeAbelianGroup σ` by transferring the property through the `equivFinsupp` isomorphism |

## Subdirectories

None.

## Search Tags

free-abelian-group finsupp isomorphism support coefficient unique-sums group-theory formal-sums finitely-supported-functions
