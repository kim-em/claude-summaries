---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/List
generated: 2025-12-09T18:35:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: preliminary
files_count: 60
subdirs_count: 1
---

# List

## Overview

The `List/` directory contains comprehensive theory and operations for lists (inductive sequences) in Lean. It provides fundamental definitions, basic properties, structural predicates (chains, cycles, duplicates, no-duplicates), list transformations (sorting, permutations, rotations, deduplication), operations on list elements (insertion, removal, indexing, splitting, zipping), and specialized constructs like association lists and list comprehensions. This foundational collection theory supports both computational list operations and formal reasoning about sequences.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions on lists including `getI`, `headI`, `getLastI` and basic operations (no proofs) |
| Basic.lean | Fundamental properties and theorems about lists including uniqueness, append associativity, and basic lemmas |
| Lemmas.lean | Additional lemmas and properties about list operations |
| Monad.lean | Monadic operations on lists |
| AList.lean | Association lists (key-value pairs) |
| Chain.lean | Chain relation: lists where consecutive elements satisfy a binary relation `r` |
| ChainOfFn.lean | Chain properties for functions generating lists |
| Count.lean | Counting occurrences of elements in lists |
| Cycle.lean | Cycles and rotational equivalence of lists; quotient by rotation relation |
| Dedup.lean | Deduplication operations on lists |
| Destutter.lean | Removing consecutive duplicate elements |
| Duplicate.lean | Detecting and working with duplicates in lists |
| DropRight.lean | Dropping elements from the right end of lists |
| Enum.lean | Enumeration operations (pairing elements with indices) |
| FinRange.lean | Lists from finite ranges |
| Flatten.lean | Flattening nested lists |
| Forall2.lean | Binary relation between corresponding elements of two lists |
| GetD.lean | Get with default value operations |
| Indexes.lean | Finding indices of elements satisfying predicates |
| Induction.lean | Induction principles for lists |
| Infix.lean | Infix (substring) relations for lists |
| InsertIdx.lean | Inserting elements at specific indices |
| InsertNth.lean | Inserting elements at nth position (deprecated wrapper) |
| Intervals.lean | List intervals and ranges |
| Iterate.lean | Iterating functions to generate lists |
| Lattice.lean | Lattice operations on lists (inf/sup) |
| Lex.lean | Lexicographic ordering on lists |
| Lookmap.lean | Looking up and mapping over list elements |
| Map2.lean | Binary map operation over two lists |
| MinMax.lean | Minimum and maximum operations on lists |
| ModifyLast.lean | Modifying the last element of a list |
| NatAntidiagonal.lean | Natural number antidiagonals for enumeration |
| Nodup.lean | Lists with no duplicate elements |
| NodupEquivFin.lean | Equivalence between no-dup lists and finite types |
| OfFn.lean | Constructing lists from functions on `Fin n` |
| Pairwise.lean | Pairwise relations between list elements |
| Palindrome.lean | Palindrome predicate for lists |
| PeriodicityLemma.lean | Periodicity properties of lists |
| Permutation.lean | List permutations and permutation properties |
| Pi.lean | Dependent function properties for lists |
| Prime.lean | Prime-related properties for lists |
| ProdSigma.lean | Product and sigma type operations on lists |
| Range.lean | Range operations for generating numeric lists |
| ReduceOption.lean | Reducing lists of options to lists of values |
| Rotate.lean | List rotation operations |
| Sections.lean | Section operations on lists |
| Shortlex.lean | Short-lex ordering (length-lexicographic) on lists |
| Sigma.lean | Sigma type operations for lists |
| Sort.lean | Sorting algorithms including insertion sort; sorted predicates (SortedLE, SortedGE, etc.) |
| SplitBy.lean | Splitting lists by predicates |
| SplitLengths.lean | Splitting lists by length specifications |
| SplitOn.lean | Splitting lists on separator elements |
| Sublists.lean | Sublist relations and operations |
| Sym.lean | Symmetric group operations on lists |
| TFAE.lean | "The Following Are Equivalent" (TFAE) predicate for list of propositions |
| TakeDrop.lean | Taking and dropping elements from lists |
| TakeWhile.lean | Taking elements while a predicate holds |
| ToFinsupp.lean | Converting lists to finitely-supported functions |
| Triplewise.lean | Triplewise relations between consecutive triples of elements |
| Zip.lean | Zipping two lists together |

## Subdirectories

- [ ] `Perm/` - Permutation relation theory and lattice structure

## Search Tags

lists sequences inductive-types list-operations sorting permutations chains cycles duplicates deduplication rotation indexing sublists association-lists enumeration lexicographic-order pairwise-relations
