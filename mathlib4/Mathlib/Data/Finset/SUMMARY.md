---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Finset
generated: 2025-12-09T10:35:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: preliminary
files_count: 49
subdirs_count: 1
---

# Finset

## Overview

The `Finset/` directory implements finite sets in Lean, providing the core data structure for representing finite subsets with decidable membership and operations. A `Finset α` is implemented as a multiset (list up to permutation) with a proof of no duplicates, enabling both computational and mathematical reasoning. This directory contains fundamental operations (insert, erase, union, intersection), cardinality theory, image/map functions, folding operations, and specialized constructions like powersets, products, antidiagonals, and sorting. Finsets serve as the foundation for finite sums/products (big operators) and the `Fintype` type class.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `Finset α` structure definition with `val` (multiset) and `nodup` proof; membership, subset relations, and coercions to `Set α` |
| Basic.lean | Fundamental lemmas on finset operations; lattice structure (union, intersection), erase operations, and extensionality |
| Card.lean | Cardinality function `Finset.card` (notation `#s`) returning the number of elements; induction principles including strong induction and erase induction |
| Image.lean | Image and map operations: `Finset.image` (applies function then deduplicates), `Finset.map` (exploits injectivity), `filterMap`, `subtype`, and `fin` |
| Fold.lean | Folding commutative associative operations over finsets; `fold op b f s` computes `f a₁ op f a₂ op ... op b` |
| Insert.lean | Insert operation and its properties for adding elements to finsets |
| Filter.lean | Filtering finsets by predicates; constructs subsets satisfying given conditions |
| Range.lean | Construction of range finsets `Finset.range n = {0, 1, ..., n-1}` |
| Attach.lean | Attaching membership proofs: converts `Finset α` to `Finset {x // x ∈ s}` |
| BooleanAlgebra.lean | Boolean algebra structure on finsets: complement operations and properties |
| Disjoint.lean | Disjointness relations between finsets |
| SDiff.lean | Set difference operation `s \ t` for finsets |
| Empty.lean | Properties of the empty finset and emptiness predicates |
| Erase.lean | Erase operation for removing specific elements from finsets |
| Powerset.lean | Powerset construction: the finset of all subsets of a given finset |
| Prod.lean | Product operations on finsets: Cartesian products `s ×ˢ t` |
| Sigma.lean | Dependent sum (Sigma type) operations on finsets |
| Sum.lean | Disjoint union operations on finsets over sum types |
| Pi.lean | Dependent product (Pi type) operations on finsets |
| Union.lean | Generalized union operations over families of finsets |
| Sups.lean | Supremum operations: finsets of pairwise suprema |
| Max.lean | Maximum element operations on finsets with order structures |
| Sort.lean | Sorting finsets into sorted lists |
| Sym.lean | Symmetric power operations on finsets |
| Functor.lean | Functor instance and categorical structure for finsets |
| Interval.lean | Interval operations and properties |
| NatAntidiagonal.lean | Natural number antidiagonals: `{(i,j) | i + j = n}` |
| MulAntidiagonal.lean | Multiplicative antidiagonals for divisor pairs |
| SMulAntidiagonal.lean | Scalar multiplication antidiagonals |
| NAry.lean | N-ary operations on finsets (operations on multiple finsets) |
| Pairwise.lean | Pairwise relations between elements of finsets |
| Preimage.lean | Preimage operations for finsets |
| PImage.lean | Partial image operations |
| Option.lean | Finset operations on `Option` types |
| Fin.lean | Specialized operations for finsets of `Fin n` |
| Finsupp.lean | Interaction between finsets and finitely supported functions |
| Update.lean | Update operations for modifying finset elements |
| Piecewise.lean | Piecewise function definitions using finsets |
| PiInduction.lean | Induction principles for Pi types over finsets |
| Slice.lean | Slice operations on finsets |
| SymmDiff.lean | Symmetric difference operation `s ∆ t = (s \ t) ∪ (t \ s)` |
| NoncommProd.lean | Non-commutative products over finsets (ordered products) |
| Grade.lean | Grading operations for finsets |
| Dedup.lean | Deduplication operations converting multisets to finsets |
| Density.lean | Density-related properties for finsets |
| CastCard.lean | Cardinality casting operations |
| Order.lean | Additional ordering properties and operations |
| Attr.lean | Attribute-related definitions for finsets |
| NatDivisors.lean | Finsets of natural number divisors |

## Subdirectories

- [ ] `Lattice/` - Lattice-theoretic operations: supremum/infimum folding, Pi/Prod lattice structures, and union lemmas

## Search Tags

finite-sets finset cardinality membership subset union intersection difference powerset product image map fold filter insert erase decidable combinatorics big-operators
