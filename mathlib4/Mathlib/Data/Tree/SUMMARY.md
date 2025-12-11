---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Tree
generated: 2025-12-11T09:15:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 4
subdirs_count: 0
---

# Tree

## Overview

The `Tree/` directory provides a binary tree data structure with values stored in non-leaf nodes. The tree supports O(lg n) retrieval using positional indices encoded as `PosNum` (binary numbers), where bit patterns determine the path through the tree (bit0 = left, bit1 = right). The implementation includes functor and traversable instances with proofs of lawfulness, as well as basic tree metrics (height, number of nodes/leaves). A special notation `a △ b` is provided for building `Tree Unit` (binary trees without data).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `Tree α` inductive type with `nil` and `node` constructors; `map`, `traverse`, `numNodes`, `numLeaves`, `height`, `left`, `right` operations; `△` notation for `Tree Unit`; proofs of functor laws and tree metric properties |
| Get.lean | Index-based retrieval operations: `indexOf` (search using decidable order), `get` (retrieve by `PosNum` path), `getOrElse` (with default value); depends on `Num` for `PosNum` type |
| RBMap.lean | Bridge to Batteries' `RBNode` type; currently minimal, with TODO to implement `Traversable` instance (though this is now in Traversable.lean) |
| Traversable.lean | `Traversable` and `LawfulTraversable` instances for `Tree`; proves composition, naturality, and identity laws for traversal |

## Subdirectories

*(none)*

## Search Tags

tree binary-tree data-structure traversable functor positional-index tree-metrics height nodes leaves
