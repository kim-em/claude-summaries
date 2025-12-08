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

- [ ] `Analysis/` - Analysis-related data structures (pending)
- [ ] `Array/` - Arrays and array operations (pending)
- [ ] `Bool/` - Boolean type properties and operations (pending)
- [ ] `Complex/` - Complex numbers ℂ (pending)
- [ ] `Countable/` - Countable types and countability properties (pending)
- [ ] `DFinsupp/` - Dependent functions with finite support (pending)
- [ ] `DList/` - Difference lists (efficient list concatenation) (pending)
- [ ] `ENNReal/` - Extended non-negative reals [0, ∞] (pending)
- [ ] `ENat/` - Extended natural numbers ℕ ∪ {∞} (pending)
- [ ] `EReal/` - Extended reals [-∞, ∞] (pending)
- [ ] `FP/` - Floating-point numbers (pending)
- [ ] `Fin/` - Finite types `Fin n` (natural numbers less than n) (pending)
- [ ] `FinEnum/` - Finitely enumerable types (pending)
- [ ] `Finite/` - Finite types and finiteness properties (pending)
- [ ] `Finset/` - Finite sets (sets with decidable membership and finite cardinality) (pending)
- [ ] `Finsupp/` - Functions with finite support (pending)
- [ ] `Fintype/` - Types with finitely many elements (pending)
- [ ] `FunLike/` - Type class for function-like structures (pending)
- [ ] `Int/` - Integers ℤ (pending)
- [ ] `List/` - Lists (inductive sequences) (pending)
- [ ] `Matrix/` - Matrices and matrix operations (pending)
- [ ] `Multiset/` - Multisets (sets with multiplicities, quotients of lists) (pending)
- [ ] `NNRat/` - Non-negative rationals ℚ≥0 (pending)
- [ ] `NNReal/` - Non-negative reals ℝ≥0 (pending)
- [ ] `Nat/` - Natural numbers ℕ (pending)
- [ ] `Num/` - Binary representation of natural numbers (pending)
- [ ] `Option/` - Option type (values that may be none) (pending)
- [ ] `Ordering/` - Ordering relation (LT, EQ, GT) (pending)
- [ ] `Ordmap/` - Ordered maps (binary search trees) (pending)
- [ ] `PFunctor/` - Polynomial functors (pending)
- [ ] `PNat/` - Positive natural numbers ℕ+ (pending)
- [ ] `PSigma/` - Dependent pairs (Sigma types) with universe flexibility (pending)
- [ ] `Pi/` - Dependent function types (Π-types) (pending)
- [ ] `Prod/` - Product types (pairs) (pending)
- [ ] `QPF/` - Quotients of polynomial functors (pending)
- [ ] `Rat/` - Rational numbers ℚ (pending)
- [ ] `Real/` - Real numbers ℝ (pending)
- [ ] `Rel/` - Relations and relation operations (pending)
- [ ] `Seq/` - Sequences (infinite lists) (pending)
- [ ] `Set/` - Sets and set operations (pending)
- [ ] `SetLike/` - Type class for set-like structures (pending)
- [ ] `Setoid/` - Setoids (types with equivalence relations) (pending)
- [ ] `Sigma/` - Dependent pairs (Sigma types) (pending)
- [ ] `Sign/` - Sign type (positive, zero, negative) (pending)
- [ ] `Stream/` - Streams (infinite sequences) (pending)
- [ ] `String/` - Strings and string operations (pending)
- [ ] `Sum/` - Sum types (disjoint unions) (pending)
- [ ] `Sym/` - Symmetric powers (pending)
- [ ] `Tree/` - Tree data structures (pending)
- [ ] `Vector/` - Vectors (lists with statically-known length) (pending)
- [ ] `W/` - W-types (well-founded trees) (pending)
- [ ] `WSeq/` - Weak sequences (potentially infinite computations) (pending)
- [ ] `ZMod/` - Integers modulo n (ℤ/nℤ) (pending)

## Search Tags

data-structures numeric-types collections lists sets multisets finsets natural-numbers integers rationals reals complex finite-types partial-functions quotients bundles opposites vectors matrices sequences
