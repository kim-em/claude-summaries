---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/BigOperators/Group/List
generated: 2025-12-01T12:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# List

## Overview

The `List/` directory provides the foundational layer for big operators over lists, implementing `List.prod` and `List.sum` along with their alternating variants `List.alternatingProd` and `List.alternatingSum`. These are the most primitive big operators in the hierarchy, operating on ordered sequences before being lifted to `Multiset` (unordered with multiplicity) and `Finset` (finite sets). The files are organized by dependency: `Defs.lean` contains the core definitions and minimal theorems, `Basic.lean` provides essential results about homomorphisms and structural properties, and `Lemmas.lean` contains advanced theorems about permutations, rotations, telescoping products, unit calculations, divisibility, and operations on opposite monoids.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of `List.prod`, `List.sum`, `List.alternatingProd`, `List.alternatingSum` with basic induction principles and initial theorems for monoids |
| Basic.lean | Fundamental theorems about list products: homomorphism preservation, relation lifting, products of maps, take/drop operations, element-wise operations, commutation, range products, and cancellation laws for groups |
| Lemmas.lean | Advanced results: permutation invariance, rotation preservation, telescoping sums/products, unit detection, divisibility from sublists, alternating product theorems, opposite monoid behavior, count-based formulas, flattening operations, and modular arithmetic preservation |

## Subdirectories

*(No subdirectories)*

## Search Tags

list-product list-sum alternating-product alternating-sum big-operators monoid group commutative-group homomorphism permutation rotation telescoping divisibility foldr ordered-sequences mathlib4-algebra
