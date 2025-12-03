---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/BigOperators/Group
generated: 2025-12-01T18:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 0
subdirs_count: 3
---

# Group

## Overview

The `Group/` directory contains the fundamental three-layer infrastructure for big operators (sums and products) over group-like algebraic structures in mathlib4. It implements a carefully stratified hierarchy where each layer builds on the previous: `List` provides the foundational definitions for ordered sequences, `Multiset` handles the quotient by permutation equivalence to achieve order-independence while preserving multiplicity, and `Finset` provides the final user-facing interface for finite sets without duplicates. This architectural design reflects deep mathematical principles: `List.prod` is defined recursively via `foldr`, `Multiset.prod` is defined as a quotient lift of `List.prod` with proofs of permutation-invariance, and `Finset.prod` is defined by mapping over the underlying multiset. The result is the standard mathematical notation `∏ i ∈ s, f i` and `∑ i ∈ s, f i` used pervasively throughout mathlib for indexed operations over commutative monoids. Beyond core definitions, the directory includes alternating products/sums, comprehensive theorems about homomorphisms and structural properties, and specialized results for powersets, sigma types, Pi types, intervals, indicator functions, piecewise functions, and preimages.

## Key Files

*(No files directly in this directory - all content is organized in subdirectories)*

## Subdirectories

- [x] `List/` - Big operators for lists: `List.prod`, `List.sum`, and alternating products/sums (`List.alternatingProd`, `List.alternatingSum`), fundamental definitions and theorems for ordered sequences including homomorphisms, permutations, rotations, telescoping products, and divisibility (3 files: Defs, Basic, Lemmas)
- [x] `Multiset/` - Big operators for multisets: `Multiset.prod` and `Multiset.sum` for unordered collections with multiplicity, quotient-based definitions via `foldr` with permutation-invariance proofs, intermediate layer handling transition from ordered to unordered aggregation (2 files: Defs, Basic)
- [x] `Finset/` - Big operators for finite sets: `Finset.prod` and `Finset.sum` with user-facing notation `∏ i ∈ s, f i` and `∑ i ∈ s, f i`, comprehensive library including specialized operations over powersets, sigma types, Pi types, intervals, indicator functions, piecewise functions, and preimages (10 files covering all major use cases)

## Search Tags

big-operators group commutative-monoid finset multiset list product sum finset-prod finset-sum list-prod list-sum multiset-prod notation hierarchy algebraic-structures ordered-sequences unordered-collections quotient foldr permutation-invariance alternating-product telescoping homomorphism powerset sigma-type pi-type indicator piecewise interval indexed-operators mathlib4-foundations
