---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Pointwise
generated: 2025-12-01T22:45:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 0
subdirs_count: 2
---

# Pointwise

## Overview

The `Pointwise/` directory provides a comprehensive theory of pointwise algebraic operations on both infinite sets (`Set`) and finite sets (`Finset`), enabling set-theoretic computations with group operations. The fundamental idea is to lift algebraic operations from elements to collections: given sets `s` and `t`, operations like `s * t` (the set of all products `x * y` where `x ∈ s` and `y ∈ t`), `s⁻¹` (pointwise inversion), `s + t` (pointwise addition), `s / t` (pointwise division), and scalar operations like `a • s` (scalar multiplication) are defined and equipped with appropriate algebraic structure instances. The development provides algebraic instances (making `Set α` and `Finset α` into semigroups/monoids/groups when `α` is), integration with big operators (products and sums), finiteness and cardinality analysis, lattice properties (unions/intersections), density preservation, interval arithmetic, and universe size constraints. All instances are carefully placed in the `Pointwise` scope to avoid conflicts with the natural monoid structure on sets and finsets.

## Key Files

No files directly in this directory; all content is organized into subdirectories.

## Subdirectories

- [x] `Finset/` - Pointwise operations on finite sets with 5 files: Basic definitions, big operators, density preservation, interval arithmetic, and scalar actions
- [x] `Set/` - Pointwise operations on infinite sets with 8 files: Basic definitions, scalar operations, lattice properties, finiteness, cardinality, big operators, list characterizations, and universe size

## Search Tags

pointwise-operations set-operations finset-operations pointwise-multiplication pointwise-addition pointwise-division pointwise-subtraction set-multiplication set-addition scalar-multiplication pointwise-scalar pointwise-inversion pointwise-negation algebraic-operations-on-sets group-operations-on-sets algebraic-instances semigroup-instance monoid-instance group-instance big-operators finiteness cardinality density lattice-operations interval-arithmetic universe-size small-instances locally-finite-order indexed-unions indexed-intersections
