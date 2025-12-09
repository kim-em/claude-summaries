---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Multiset
generated: 2025-12-09T10:00:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: preliminary
files_count: 29
subdirs_count: 0
---

# Multiset

## Overview

The `Multiset/` directory implements multisets (finite sets with duplicates allowed) as quotients of lists by permutation equivalence. This provides a computationally-meaningful data structure where element order doesn't matter but multiplicity does. The implementation includes core definitions, constructors (empty, cons, singleton), counting and membership predicates, monadic operations (bind, join, product), set-like operations (union, intersection, powerset), folding and mapping functions, sorting, lattice operations, and specialized utilities for intervals, antidiagonals, and symmetric powers. The design carefully avoids dependencies on algebra to keep this foundational layer lightweight.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Multiset α` as quotient of `List α` by permutation; includes basic predicates like membership, subset, partial order, pairwise, and nodup |
| ZeroCons.lean | Constructors for multisets: empty multiset (0), cons operation (::ₘ), singleton; defines `Multiset.Rel` for lifting relations between elements to multisets; includes recursion principle |
| Basic.lean | Basic results on multisets including `toList` conversion, induction principles (strong induction, strong downward induction) |
| Count.lean | Counting multiplicity: `countP` for counting elements satisfying a predicate, `count` for counting specific elements |
| Bind.lean | Monadic operations: `join` (flatten multiset of multisets), `bind` (monadic bind), `product` (cartesian product), `sigma` (disjoint sum in sigma types) |
| FinsetOps.lean | Operations that ignore multiplicities in preparation for `Finset`: `ndinsert` (insert ignoring duplicates), `ndinter` (intersection), `ndunion` (union), `erase_dup` |
| Dedup.lean | Deduplication operation that removes duplicate elements from a multiset |
| Filter.lean | Filter operation for multisets with decidable predicates |
| Fold.lean | Folding operations on multisets with associative-commutative operators |
| MapFold.lean | Combined map and fold operations for multisets |
| Lattice.lean | Lattice operations: `sup` (supremum), `inf` (infimum) for multisets over lattice types |
| UnionInter.lean | Union and intersection operations respecting multiplicities (max and min of counts) |
| AddSub.lean | Addition and subtraction operations on multisets (sum and difference of multiplicities) |
| Powerset.lean | Powerset operation: all sub-multisets of a given multiset |
| Antidiagonal.lean | Antidiagonal operation: all pairs of multisets `(t₁, t₂)` such that `t₁ + t₂ = s` |
| NatAntidiagonal.lean | Antidiagonal for natural numbers (specialized version) |
| Sort.lean | Sorting multisets to produce ordered lists using merge sort algorithm |
| Range.lean | Range operation for creating multisets of consecutive numbers |
| Replicate.lean | Replicate operation: create multiset with n copies of an element |
| Interval.lean | Interval operations on multisets |
| Pi.lean | Pi-type (dependent function) operations on multisets |
| Sections.lean | Sections of multiset-valued functions |
| Sum.lean | Sum operations on multisets |
| Sym.lean | Connection to symmetric powers (Sym types) |
| Pairwise.lean | Pairwise relation predicates on multisets |
| Fintype.lean | Finiteness properties: instances showing multisets are fintype when base type is fintype |
| Functor.lean | Functor instance for multisets (for applicative/monad infrastructure) |
| OrderedMonoid.lean | Ordered monoid instances for multisets |
| DershowitzManna.lean | Dershowitz-Manna multiset ordering (well-founded ordering on multisets) |

## Subdirectories

*(none)*

## Search Tags

multiset quotient list permutation multiplicity counting membership subset cons join bind product powerset antidiagonal fold filter map lattice union intersection sort finset deduplication
