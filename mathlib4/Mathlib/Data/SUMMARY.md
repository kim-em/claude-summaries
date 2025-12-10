---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 24
subdirs_count: 54
---

# Data

## Overview

The `Data/` directory contains fundamental data structures, numeric types, and type-level constructs that serve as the foundation for mathematical reasoning in mathlib4. It encompasses concrete implementations of natural numbers, integers, rationals, reals, complex numbers, finite types, collections (lists, sets, multisets, finsets), partial/dependent functions, and specialized mathematical constructs like quotients, bundles, and opposites. These implementations provide both computational content and the algebraic/order-theoretic properties needed for formal mathematics, bridging between Lean's core types and mathlib's rich mathematical hierarchy.

## Key Files

| File | Purpose |
|------|---------|
| BitVec.lean | Additional theorems about bitvectors (bit vectors of fixed width) that depend on Mathlib; includes integer casting, injectivity properties |
| Bracket.lean | Bracket notation and operations for mathematical expressions |
| Bundle.lean | Basic data structure for fiber bundles and vector bundles; defines `Bundle.TotalSpace` as dependent type pairs `⟨b, x⟩` where `b : B` and `x : E b` |
| Char.lean | `LinearOrder` instance on `Char` (Unicode scalar values) and `UInt8` truncation |
| Erased.lean | Type `Erased α` that is classically isomorphic to `α` but erased in the VM at runtime (represented as 0 like proofs); used for tracking data without storing it |
| FinEnum.lean | Type class `FinEnum α` for finitely enumerable types with explicit bijection to `Fin n`; stronger than `Fintype` by assigning ranks |
| Finmap.lean | Finite maps over `Multiset`; association lists with operations on keys and values |
| Holor.lean | Higher-order tensor-like objects (holors) |
| Ineq.lean | Inequality constructs and operations |
| Opposite.lean | Structure `Opposite α` (notation `αᵒᵖ`) with bijections `op : α → αᵒᵖ` and `unop : αᵒᵖ → α`; used for opposite categories |
| PEquiv.lean | Partial equivalences (notation `≃.`): bijections between subsets of types, stored as functions `α → Option β` and `β → Option α` |
| PFun.lean | Partial functions `α →. β` defined as `α → Part β`; includes domain, evaluation, composition, restriction, and fixed-point operations |
| Part.lean | Partial values `Part α`: values with a domain proposition and getter function; behaves like `Option α` but domain need not be decidable |
| Quot.lean | Extensions to core library's quotient types; additional operations and properties for quotients and setoids |
| Rel.lean | Relations between types and operations on relations |
| SProd.lean | Strict product types |
| Semiquot.lean | Semiquotient types (partial quotients) |
| Subtype.lean | API for subtypes `{val : α // p val}`; pairs of values with proofs of predicates, with coercion to parent type |
| TwoPointing.lean | Types with two distinguished points |
| TypeVec.lean | Type vectors for representing families of types |
| UInt.lean | Unsigned integer types and operations |
| ULift.lean | Universe lifting for types; allows moving types between universes |
| Vector3.lean | 3-dimensional vectors |

## Subdirectories

- [x] `Analysis/` - Computational realization of filters and topological spaces (experimental infrastructure for computing with analysis concepts)
- [x] `Array/` - Arrays and array operations
- [x] `Bool/` - Boolean type properties and operations
- [ ] `Complex/` - Complex numbers ℂ
- [x] `Countable/` - Countable types and countability properties
- [x] `DFinsupp/` - Dependent functions with finite support
- [x] `DList/` - Difference lists (efficient list concatenation)
- [x] `ENNReal/` - Extended non-negative reals [0, ∞]
- [x] `ENat/` - Extended natural numbers ℕ ∪ {∞}
- [x] `EReal/` - Extended reals [-∞, ∞]
- [x] `FP/` - Floating-point numbers
- [x] `Fin/` - Finite types `Fin n` (natural numbers less than n)
- [x] `FinEnum/` - Finitely enumerable types
- [x] `Finite/` - Finite types and finiteness properties
- [x] `Finset/` - Finite sets (sets with decidable membership and finite cardinality)
- [x] `Finsupp/` - Functions with finite support
- [x] `Fintype/` - Types with finitely many elements
- [x] `FunLike/` - Type class for function-like structures
- [x] `Int/` - Integers ℤ
- [x] `List/` - Lists (inductive sequences)
- [x] `Matrix/` - Matrices and matrix operations
- [x] `Multiset/` - Multisets (sets with multiplicities, quotients of lists)
- [x] `NNRat/` - Non-negative rationals ℚ≥0
- [x] `NNReal/` - Non-negative reals ℝ≥0
- [x] `Nat/` - Natural numbers ℕ
- [x] `Num/` - Binary representation of natural numbers
- [x] `Option/` - Option type (values that may be none)
- [ ] `Ordering/` - Ordering relation (LT, EQ, GT)
- [ ] `Ordmap/` - Ordered maps (binary search trees)
- [ ] `PFunctor/` - Polynomial functors
- [ ] `PNat/` - Positive natural numbers ℕ+
- [ ] `PSigma/` - Dependent pairs (Sigma types) with universe flexibility
- [ ] `Pi/` - Dependent function types (Π-types)
- [ ] `Prod/` - Product types (pairs)
- [ ] `QPF/` - Quotients of polynomial functors
- [ ] `Rat/` - Rational numbers ℚ
- [ ] `Real/` - Real numbers ℝ
- [ ] `Rel/` - Relations and relation operations
- [ ] `Seq/` - Sequences (infinite lists)
- [ ] `Set/` - Sets and set operations
- [ ] `SetLike/` - Type class for set-like structures
- [ ] `Setoid/` - Setoids (types with equivalence relations)
- [ ] `Sigma/` - Dependent pairs (Sigma types)
- [ ] `Sign/` - Sign type (positive, zero, negative)
- [ ] `Stream/` - Streams (infinite sequences)
- [ ] `String/` - Strings and string operations
- [ ] `Sum/` - Sum types (disjoint unions)
- [ ] `Sym/` - Symmetric powers
- [ ] `Tree/` - Tree data structures
- [ ] `Vector/` - Vectors (lists with statically-known length)
- [ ] `W/` - W-types (well-founded trees)
- [ ] `WSeq/` - Weak sequences (potentially infinite computations)
- [ ] `ZMod/` - Integers modulo n (ℤ/nℤ)

## Search Tags

data-structures numeric-types collections lists sets multisets finsets natural-numbers integers rationals reals complex finite-types partial-functions quotients bundles opposites vectors matrices sequences
