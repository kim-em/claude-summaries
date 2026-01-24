---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data
generated: 2026-01-24T12:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 24
subdirs_count: 54
---

# Data

## Overview

The `Data/` directory is mathlib4's foundational layer for data structures, numeric types, and type-level constructs—the infrastructure upon which formal mathematics is built. This comprehensive directory (54 subdirectories, 24 top-level files) provides:

**Numeric tower**: The complete hierarchy from natural numbers (`Nat/`) through integers (`Int/`), rationals (`Rat/`), and reals (`Real/`) to complex numbers (`Complex/`), plus specialized variants including positive naturals (`PNat/`), non-negative reals/rationals (`NNReal/`, `NNRat/`), and extended types with infinity (`ENat/`, `ENNReal/`, `EReal/`). Each includes arithmetic operations, order structures, and algebraic instances.

**Finite structures**: Three complementary notions of finiteness—`Fintype` (computational, enumerable), `Finite` (propositional, proof-irrelevant), and `FinEnum` (with explicit bijection to `Fin n`)—plus the workhorse `Finset` for decidable finite sets and `Fin` for bounded natural numbers with comprehensive tuple/vector support.

**Collections**: Lists (`List/`) as the foundational sequence type with 60+ files covering chains, cycles, permutations, and sorting; multisets (`Multiset/`) as lists quotiented by permutation; sets (`Set/`) as predicates with complete Boolean algebra structure; and specialized ordered maps (`Ordmap/`) as verified binary search trees.

**Sparse/dependent functions**: `Finsupp` for finitely-supported functions (foundation for polynomials and monoid algebras) and `DFinsupp` for dependent functions with finite support, both with comprehensive algebraic and order structures.

**Coinductive types**: Sequences (`Seq/`) and weak sequences (`WSeq/`) for possibly-infinite lists, computations (`Computation`) for unbounded computations, and streams (`Stream/`) for infinite sequences.

**Categorical constructions**: Polynomial functors (`PFunctor/`) and their quotients (`QPF/`) for defining inductive/coinductive types; W-types (`W/`) for well-founded trees; opposites (`Opposite`) for dual categories; and type vectors (`TypeVec`) for multivariate functors.

**Type-theoretic infrastructure**: Partial functions (`Part`, `PFun`, `PEquiv`), quotients (`Quot`, `Setoid/`), universe lifting (`ULift`), subtypes (`Subtype`), sigma types (`Sigma/`, `PSigma/`), product types (`Prod/`), sum types (`Sum/`), and function-like typeclasses (`FunLike/`).

**Modular arithmetic**: `ZMod` for integers mod n with field structure for prime moduli, Chinese Remainder Theorem, and quotient group/ring equivalences.

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
- [x] `Complex/` - Complex numbers ℂ: field structure, imaginary unit, conjugation, norm squared
- [x] `Countable/` - Countable types and countability properties
- [x] `DFinsupp/` - Dependent functions with finite support (`Π₀ i, β i`)
- [x] `DList/` - Difference lists (efficient list concatenation)
- [x] `ENNReal/` - Extended non-negative reals [0, ∞] for measure theory
- [x] `ENat/` - Extended natural numbers ℕ ∪ {∞}
- [x] `EReal/` - Extended reals [-∞, ∞]
- [x] `FP/` - Floating-point numbers (experimental)
- [x] `Fin/` - Finite types `Fin n` (natural numbers less than n) with tuple/vector support
- [x] `FinEnum/` - Finitely enumerable types with Option recursor
- [x] `Finite/` - Finite types (propositional, proof-irrelevant)
- [x] `Finset/` - Finite sets with decidable membership, cardinality, and lattice operations
- [x] `Finsupp/` - Functions with finite support (`α →₀ M`) for polynomials and algebras
- [x] `Fintype/` - Types with finitely many elements (computational enumeration)
- [x] `FunLike/` - Type class for function-like structures (homomorphisms, embeddings, equivalences)
- [x] `Int/` - Integers ℤ with GCD, modular arithmetic, Bézout's lemma
- [x] `List/` - Lists (inductive sequences) with 60+ files covering chains, permutations, sorting
- [x] `Matrix/` - Matrices and matrix operations
- [x] `Multiset/` - Multisets (sets with multiplicities, quotients of lists)
- [x] `NNRat/` - Non-negative rationals ℚ≥0
- [x] `NNReal/` - Non-negative reals ℝ≥0
- [x] `Nat/` - Natural numbers ℕ with factorization, primality, combinatorics, digits
- [x] `Num/` - Binary representation of natural numbers (PosNum, Num, ZNum)
- [x] `Option/` - Option type (values that may be none)
- [x] `Ordering/` - Ordering relation (LT, EQ, GT) and comparison functions
- [x] `Ordmap/` - Ordered maps (verified weight-balanced binary search trees)
- [x] `PFunctor/` - Polynomial functors for inductive/coinductive types
- [x] `PNat/` - Positive natural numbers ℕ+ with factorization and extended GCD
- [x] `PSigma/` - Dependent pairs (Sigma types) with universe flexibility and lexicographic order
- [x] `Pi/` - Dependent function types (Π-types) with locally finite order instances
- [x] `Prod/` - Product types (pairs) with lexicographic ordering
- [x] `QPF/` - Quotients of polynomial functors for advanced inductive types
- [x] `Rat/` - Rational numbers ℚ with floor/ceiling, encodability, cardinality
- [x] `Real/` - Real numbers ℝ as Cauchy sequences with Archimedean property
- [x] `Rel/` - Relations: separation and covering for uniform spaces
- [x] `Seq/` - Sequences (possibly infinite lists) and parallel computation
- [x] `Set/` - Sets and set operations with complete Boolean algebra structure
- [x] `SetLike/` - Type class for set-like structures (submonoids, submodules, etc.)
- [x] `Setoid/` - Setoids (types with equivalence relations) and partitions
- [x] `Sigma/` - Dependent pairs (Sigma types) with disjoint sum and lexicographic orders
- [x] `Sign/` - Sign type (positive, zero, negative) with CommGroupWithZero structure
- [x] `Stream/` - Streams (infinite sequences) with coinduction and bisimulation
- [x] `String/` - Strings and string operations with linear order
- [x] `Sum/` - Sum types (disjoint unions) with lexicographic and disjoint orders
- [x] `Sym/` - Symmetric powers (unordered tuples) with stars-and-bars combinatorics
- [x] `Tree/` - Tree data structures with traversable functor instances
- [x] `Vector/` - Vectors (lists with statically-known length) for mathematical reasoning
- [x] `W/` - W-types (well-founded trees) with encodability and cardinality
- [x] `WSeq/` - Weak sequences (potentially infinite computations with thinking steps)
- [x] `ZMod/` - Integers modulo n (ℤ/nℤ) with field structure for primes

## Search Tags

data-structures numeric-types collections lists sets multisets finsets natural-numbers integers rationals reals complex finite-types partial-functions quotients bundles opposites vectors matrices sequences polynomials finitely-supported-functions dependent-types coinductive w-types streams computations modular-arithmetic polynomial-functors
