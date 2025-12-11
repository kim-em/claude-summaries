---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Sum
generated: 2025-12-11T10:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 4
subdirs_count: 0
---

# Sum

## Overview

The `Sum/` directory provides comprehensive order-theoretic infrastructure for sum types (disjoint unions) `α ⊕ β`. It defines two main orderings: the **disjoint sum** where elements from different summands are incomparable, and the **lexicographic sum** `α ⊕ₗ β` where all elements of `α` are less than all elements of `β`. The directory includes instances for preorders, partial orders, linear orders, lattices, and locally finite orders, along with utilities for lifting relations, computing finite intervals, and establishing order isomorphisms.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Additional lemmas about sum types beyond Batteries; includes function update lemmas for `Sum.elim`, injectivity/surjectivity of `Sum.map`, `LiftRel` utilities, ternary sum abbreviations (`Sum3.in₀/in₁/in₂`), and `PSum` injectivity lemmas |
| Order.lean | Defines disjoint sum orders (`Sum.LE`, `Sum.LT`) via `LiftRel` and lexicographic sum orders (`Sum.Lex.LE`, `Sum.Lex.LT`); provides `Preorder`, `PartialOrder`, `LinearOrder` instances; includes `NoMinOrder`, `NoMaxOrder`, `DenselyOrdered` instances; defines order isomorphisms (`sumCongr`, `sumComm`, `sumAssoc`, `sumDualDistrib`, `sumLexCongr`, `sumLexDualAntidistrib`); establishes `WithBot`/`WithTop` isomorphisms to lexicographic sums |
| Lattice.lean | Lattice structure for lexicographic sums `α ⊕ₗ β`; provides `SemilatticeSup`, `SemilatticeInf`, `Lattice`, and `DistribLattice` instances; defines `inlLatticeHom` and `inrLatticeHom` as lattice homomorphisms |
| Interval.lean | `LocallyFiniteOrder` instances for sum types; defines `sumLift₂` and `sumLexLift` for lifting interval operations; computes finite intervals `Icc`, `Ico`, `Ioc`, `Ioo` for both disjoint and lexicographic sums; provides `LocallyFiniteOrderBot` and `LocallyFiniteOrderTop` instances |

## Subdirectories

(none)

## Search Tags

sum-types disjoint-union coproduct lexicographic-order order-theory lift-rel locally-finite-order interval lattice semilattice order-isomorphism with-bot with-top inl inr
