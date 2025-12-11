---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Set
generated: 2025-12-11T12:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: preliminary
files_count: 38
subdirs_count: 5
---

# Set

## Overview

The `Set/` directory provides the foundational theory of sets in mathlib4, where sets are defined as predicates (`Set α := α → Prop`). This directory contains the core definitions, operations, and properties for working with sets including membership, subset relations, union, intersection, complement, image, preimage, and the complete lattice structure. It also covers specialized topics like functions on sets (injectivity, surjectivity, bijectivity restricted to sets), cardinality (both computable and noncomputable), countability, pairwise relations, and pointwise operations with algebraic structures.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `Set α := α → Prop`, `setOf`, membership, subset, empty set, insert, singleton, union, intersection, complement, difference, powerset, image, and `Nonempty` predicate |
| Basic.lean | Basic properties of sets; `DistribLattice` and `BoundedOrder` instances; fundamental lemmas for empty set, univ, union, intersection, insert, singleton, and powerset |
| Notation.lean | Scoped notation for set operations: coercion `↑` for `Set s → Set α` and `↓∩` for intersection as a set in a subtype |
| Operations.lean | Additional set operations and their properties |
| Lattice.lean | Complete atomic Boolean algebra structure on `Set α`; indexed unions/intersections (`⋃`, `⋂`), bounded unions (`biUnion`, `biInter`) |
| Image.lean | Image `f '' s` and preimage `f ⁻¹' t` operations; range of a function; lemmas for images under various operations |
| Function.lean | Predicates for functions restricted to sets: `EqOn`, `MapsTo`, `InjOn`, `SurjOn`, `BijOn`, `LeftInvOn`, `RightInvOn`, `InvOn` |
| Card.lean | Noncomputable set cardinality: `encard` (as `ℕ∞`) and `ncard` (as `ℕ` with junk value 0 for infinite sets) |
| Countable.lean | `Set.Countable s` definition (abbreviation for `Countable s`) and basic properties |
| Prod.lean | Sets in product types `α × β`; Cartesian product `s ×ˢ t`, diagonal, off-diagonal, pi sets |
| Restrict.lean | Restriction of functions to sets |
| Subset.lean | Properties of subset relation and subset-related operations |
| Insert.lean | Properties of `Set.insert` operation |
| NAry.lean | N-ary images `image2` for binary operations on sets |
| Piecewise.lean | Piecewise-defined functions on sets |
| Sups.lean | Set family operations for combinatorics: `⊻` and `⊼` for pointwise sup/inf |
| UnionLift.lean | `iUnionLift` to glue functions defined on each set of a union |
| Accumulate.lean | Accumulation of set sequences |
| BoolIndicator.lean | Boolean indicator functions for sets |
| BooleanAlgebra.lean | Boolean algebra structure on sets |
| CoeSort.lean | Coercion from sets to types (subtypes) |
| Constructions.lean | Constructions involving sets |
| Disjoint.lean | Disjointness of sets |
| Enumerate.lean | Enumeration of set elements |
| Equitable.lean | Equitable partitions of sets |
| Functor.lean | Functor instance for sets |
| Inclusion.lean | Inclusion maps between subsets |
| List.lean | Interaction between sets and lists |
| MemPartition.lean | Membership-based partitions |
| Monotone.lean | Monotone functions on sets |
| MulAntidiagonal.lean | Multiplicative antidiagonals in sets |
| Opposite.lean | Sets in opposite types |
| Order.lean | Order-theoretic properties of sets |
| Semiring.lean | Semiring-like operations on sets |
| Sigma.lean | Sets in sigma types |
| Subsingleton.lean | Subsingleton sets (sets with at most one element) |
| SymmDiff.lean | Symmetric difference of sets |

## Subdirectories

- [x] `Card/` - Arithmetic lemmas for set cardinality
- [ ] `Finite/` - Finite sets: basic properties, lattice operations, lists, monadic operations, powerset, and ranges
- [ ] `Lattice/` - Lattice operations on images of sets
- [ ] `Pairwise/` - Pairwise relations on sets: basic properties, chains, lattice operations, and list interactions
- [ ] `Pointwise/` - Pointwise algebraic operations on sets (e.g., `s * t`, `s + t` for sets in monoids/groups)

## Search Tags

set sets predicate membership subset union intersection complement difference image preimage lattice boolean-algebra cardinality countable finite injective surjective bijective pairwise pointwise
