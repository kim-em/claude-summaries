---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Partition
generated: 2026-01-26T18:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Partition

## Overview

The `Partition/` directory formalizes two notions of partitions: general partitions in complete lattices (where a partition is an independent family of nontrivial elements with a given supremum) and finite partitions of finsets (pairwise disjoint finite collections without ⊥). The directory includes specialized theory for equipartitions (finite partitions with parts of nearly equal size, differing by at most 1), with applications to combinatorics and Szemerédi's regularity lemma. All three files provide extensive APIs including constructors, refinement orders, bind operations, and connections to equivalence relations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | General partition structure for complete lattices: `Partition s` as an independent set of nontrivial elements with supremum `s`, SetLike instance, disjointness properties, copy/removeBot constructors; intended to link with Finpartition |
| Finpartition.lean | Finite partitions of elements in lattices with ⊥: `Finpartition a` structure with supremum-independent parts, refinement partial order, semilattice inf structure for distributive lattices, bind operation (monadic structure with indiscrete), discrete/indiscrete partitions, atomise construction, equivalence classes from setoids |
| Equipartition.lean | Equipartitions of finite sets: `IsEquipartition` predicate for finpartitions with parts of size `n/k` or `n/k+1`, counting theorems for large/small parts, part-preserving enumerations where indices are congruent modulo number of parts, discrete and indiscrete equipartitions |

## Subdirectories

(none)

## Search Tags

partition finpartition equipartition independent-set supremum-independent disjoint pairwise-disjoint refinement-order semilattice atomise setoid equivalence-class discrete-partition indiscrete-partition bind equitable Szemeredi-regularity complete-lattice order-bot
