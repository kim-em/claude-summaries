---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/GroupWithZero
generated: 2025-12-01T20:55:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 8
subdirs_count: 2
---

# GroupWithZero

## Overview

The `GroupWithZero/` directory provides the comprehensive theory of ordered groups and monoids with a zero element, which are fundamental structures in valuation theory and algebraic number theory. The main focus is on `LinearOrderedCommMonoidWithZero` and `LinearOrderedCommGroupWithZero`, which formalize linearly ordered commutative groups/monoids with an adjoined zero (like the target of valuations). The directory encompasses three major components: (1) core algebraic definitions and constructions (`WithZero` wrapper, canonical order instances, lexicographic products), (2) fine-grained unbundled typeclasses for multiplication monotonicity and covariance (eight granular classes like `PosMulMono` and `PosMulStrictMono`, with order isomorphisms enabling lattice distribution), and (3) infrastructure for transferring these structures to order type synonyms (`αᵒᵈ`, `Lex α`) including group action instances. Additional utilities cover finset operations, bounded sets, and positive submonoids.

## Key Files

| File | Purpose |
|------|---------|
| Canonical.lean | Core definitions of `LinearOrderedCommMonoidWithZero` and `LinearOrderedCommGroupWithZero` typeclasses, their basic properties (`zero_le`, `le_zero_iff`), order instances for dual types, dense order characterization via units, and conversions between multiplicative and additive views |
| WithZero.lean | Comprehensive `WithZero` construction adding zero to a type: order instances (preorder, partial order, linear order, lattice), covariance instances (`PosMulStrictMono`, `MulPosStrictMono`, etc.), canonical ordered structures, and exponential/logarithm order isomorphisms for `Gᵐ⁰` |
| Bounds.lean | Lemmas for bounded-above sets: `BddAbove.range_comp_of_nonneg` for composing with monotone functions on nonnegative values, and `bddAbove_range_mul` for products of nonnegative bounded functions |
| Lex.lean | Order homomorphisms for lexicographic products of linearly ordered groups with zero: natural inclusions `inl`, `inr` and projection `fst` between `α`, `β` and `WithZero (αˣ ×ₗ βˣ)`, with monotonicity and strict monotonicity properties |
| Finset.lean | Finset supremum/infimum operations in ordered monoids with zero: inequalities relating `sup (a * b)` to `sup a * sup b` for nonnegative functions, and division-preserving supremum identities using order isomorphisms (`sup'_div₀`, `sup_div₀`) |
| Submonoid.lean | Definition of the positive elements submonoid `Submonoid.pos α := Set.Ioi 0` for ordered monoids with zero |
| Synonym.lean | Transfer of group-with-zero structure to order type synonyms: instances for `αᵒᵈ` (order dual) and `Lex α` (lexicographic order) preserving all algebraic properties from `MulZeroClass` through `CommGroupWithZero` |
| Unbundled.lean | Deprecated entry point (since 2025-04-13) redirecting to `Unbundled/Basic` and `Unbundled/Defs` subdirectory files |

## Subdirectories

- [x] `Action/` - Group action with zero instances transferred to order type synonyms `αᵒᵈ` and `Lex α`, providing infrastructure for actions by and on ordered structures with zero via `SMulWithZero`, `DistribSMul`, `DistribMulAction`, and `MulActionWithZero` (complete)
- [x] `Unbundled/` - Fine-grained unbundled typeclasses for multiplication monotonicity and covariance in ordered structures with zero: eight core classes (`PosMulMono`, `PosMulStrictMono`, `PosMulReflectLT/LE` and right-multiplication counterparts), order isomorphisms for multiplication by positive elements (`OrderIso.mulLeft₀`, `mulRight₀`), and comprehensive monotonicity lemmas (complete)

## Search Tags

ordered-group-with-zero linearly-ordered-group-with-zero valuation-theory with-zero canonical-order lex-product order-homomorphism finset-supremum bounded-above positive-submonoid covariance-classes exponential-logarithm order-isomorphism dense-order units-characterization
