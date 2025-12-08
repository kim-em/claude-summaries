---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Array
generated: 2025-12-08T15:43:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Array

## Overview

The `Array/` directory provides definitions and lemmas for array operations in Lean. It contains cyclic permutation operations for rearranging array elements, and theorems about array extraction (slicing). This is a foundational directory for working with arrays beyond the core library's basic operations.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Definitions for array operations including `cyclicPermute!` (permute array using cyclic indices) and `permute!` (permute using lists of cycles) |
| Extract.lean | Lemmas about `Array.extract` (array slicing), including theorems for extracting from concatenated arrays and handling edge cases |

## Subdirectories

None.

## Search Tags

arrays data-structures permutation cyclic-permutation array-slicing extraction array-operations
