---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Pointwise/Set
generated: 2025-12-01T22:30:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 8
subdirs_count: 0
---

# Set

## Overview

The `Set/` subdirectory provides the complete theory of pointwise algebraic operations on infinite sets. It defines operations like `s * t` (the set of all products `x * y` where `x ∈ s` and `y ∈ t`), `s⁻¹` (pointwise inversion), `a • s` (scalar multiplication), and related algebraic structures. The theory includes algebraic instances (making `Set α` a semigroup/monoid when `α` is), big operator interactions (products and sums over finsets), cardinality bounds, finiteness preservation, lattice properties (unions/intersections of pointwise operations), and universe size constraints. All instances are placed in the `Pointwise` scope to avoid conflicts with the natural monoid structure on sets.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of pointwise operations (`*`, `+`, `⁻¹`, `-`, `/`, `1`, `0`) and fundamental algebraic instances for sets (semigroup, monoid, group structures) |
| Scalar.lean | Pointwise scalar operations including `a • s` (scaling/translation), `s • t` (pointwise scalar multiplication), and `s -ᵥ t` (pointwise scalar subtraction) |
| Lattice.lean | Interaction between pointwise operations and set lattice operations (indexed unions/intersections of products, sums, inversions) |
| Finite.lean | Finiteness preservation lemmas showing how pointwise operations preserve or propagate finiteness and infinity of sets |
| Card.lean | Cardinality bounds and exact cardinality formulas for pointwise operations using cardinal arithmetic and natural cardinalities |
| BigOperators.lean | Integration with big operators: how pointwise products/sums interact with finite products/sums (finset prod, multiset prod, list prod) |
| ListOfFn.lean | Characterization of membership in products of lists of sets and powers of sets using functions from `Fin n` |
| Small.lean | Universe size preservation (`Small` instances) showing that pointwise operations preserve small sets in a given universe |

## Subdirectories

(No subdirectories)

## Search Tags

pointwise-operations set-operations pointwise-multiplication pointwise-addition set-multiplication set-addition scalar-multiplication pointwise-scalar inversion negation division subtraction algebraic-instances semigroup-instance monoid-instance group-instance finiteness cardinality big-operators lattice-operations indexed-unions indexed-intersections universe-size small-instances
