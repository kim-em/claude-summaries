---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Filter/Germ
generated: 2026-01-26T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Germ

## Overview

The `Germ/` directory formalizes germs of functions at a filter. A germ is an equivalence class of functions `α → β` under the relation "eventually equal" with respect to a filter `l`: two functions are equivalent if they agree on a filter neighborhood. This construction is fundamental in analysis for studying local behavior of functions near points, at infinity, or in measure-theoretic contexts (almost everywhere). The directory provides the core `Germ l β` type as a quotient, operations on germs (map, map₂, composition, tendsto), lifting of predicates and relations, and comprehensive algebraic structure: germs inherit algebraic operations pointwise from the target type, including group, ring, module, and lattice structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core germ theory: `Germ l β` definition as quotient by `EventuallyEq l`; dependent version `Product l ε` for Pi types; map/map₂ operations; `IsConstant` predicate; composition with functions tending to the filter (`compTendsto`, `compTendsto'`); lifting predicates/relations (`LiftPred`, `LiftRel`); comprehensive algebraic instances (Semigroup, Monoid, Group, CommGroup, MulZeroClass, Semiring, Ring, CommRing, Module, MulAction); order structures (PartialOrder, Lattice, DistribLattice, BoundedOrder); coercion from functions and constants |
| OrderedMonoid.lean | Ordered monoid structures on germs: instances for `IsOrderedMonoid`, `IsOrderedCancelMonoid`, and `CanonicallyOrderedMul` when the target type has these structures; complements Basic.lean with order-compatible multiplication |

## Subdirectories

(none)

## Search Tags

germ eventually-equal quotient filter local-behavior analysis EventuallyEq Tendsto map map₂ LiftPred LiftRel algebraic-structure pointwise-operations module ring lattice partial-order composition almost-everywhere neighborhood
