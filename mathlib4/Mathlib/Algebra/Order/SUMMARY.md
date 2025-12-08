---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order
generated: 2025-12-01T22:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 21
subdirs_count: 20
---

# Order

## Overview

The `Order/` directory synthesizes algebra and order theory into a unified framework for ordered algebraic structures. At its core, it establishes how algebraic operations (addition, multiplication, scalar actions) interact with ordering relations across the full spectrum of algebraic hierarchy: from basic monoids through groups, rings, modules, to fields. The directory provides both **bundled typeclasses** (e.g., `OrderedRing`, `LinearOrderedField`) that package structure and order together, and **unbundled approaches** using fine-grained covariance/contravariance typeclasses (e.g., `CovariantClass`, `PosMulMono`) for precise control over monotonicity assumptions.

Beyond definitional infrastructure, the directory develops substantial mathematical theory: the **Hahn embedding theorem** for linearly ordered modules into Hahn series, **Cauchy sequence completions** constructing ℝ and p-adic numbers, **floor and ceiling functions** with Galois characterizations, **archimedean theory** including uniqueness of field homomorphisms and archimedean classes, and classical inequalities (**Bernoulli**, **Cauchy-Schwarz**, **Chebyshev**, **rearrangement**). Specialized constructions include **Kleene algebras** for computability, **quantales** for non-commutative logic, **absolute values** (both bundled and unbundled), **interval arithmetic** across multiple container types (finsets, multisets, sets), and comprehensive subtype theories for **nonnegative** and **positive** elements that enable working with types like `ℝ≥0` as first-class algebraic objects.

The directory's organization reflects mathematical stratification: core structures (`Group/`, `Monoid/`, `Ring/`, `Field/`, `Module/`) provide foundations; specialized constructions (`WithTop/`, `WithBot/`, `GroupWithZero/`) handle adjoined elements for valuation theory; and utility modules (`Floor/`, `Hom/`, `BigOperators/`, `Interval/`) provide computational and homomorphism infrastructure. Throughout, the emphasis is on **compatibility lemmas** showing how order interacts with algebraic operations, enabling systematic verification of order-preserving calculations.

## Key Files

| File | Purpose |
|------|---------|
| ZeroLEOne.lean | Typeclass `ZeroLEOneClass` expressing `0 ≤ 1`, with instances for `Nat`, `Int`, `Rat`, and product/Pi types |
| Algebra.lean | Ordered algebras: ordered semirings that are algebras over ordered commutative semirings with compatible scalar multiplication |
| Kleene.lean | Idempotent semirings and Kleene algebras for computability theory: defines `IdemSemiring`, `IdemCommSemiring`, `KleeneAlgebra` with Kleene star operator satisfying fixed-point axioms `1 + a * aˢᵗᵃʳ ≤ aˢᵗᵃʳ` |
| Quantale.lean | Quantales: semigroups distributing over complete lattices `x * (⨆ i, f i) = ⨆ i, x * f i`, with left/right residuation operators `x ⇨ y` and `y ⇦ x` for non-commutative logic |
| CompleteField.lean | Complete ordered fields: fields with Dedekind-complete ordering where every bounded set has supremum/infimum, generalizing ℝ |
| Rearrangement.lean | Rearrangement inequality: `∑ i, f i * g (σ i)` maximized when `g ∘ σ` monovaries with `f`, minimized when they antivary |
| Monovary.lean | Interaction of ordered algebraic structures with monovariance/antivariance: defines when two functions "move together" or "move opposite" preserving order relationships |
| Chebyshev.lean | Chebyshev's sum inequality: `(∑ i, f i) * (∑ i, g i) ≤ #s * ∑ i, f i * g i` when `f` and `g` monovary, with duality for antivariance |
| Floor.lean | Deprecated entry point for floor/ceiling function theory (redirects to `Floor/` subdirectory containing FloorSemiring and FloorRing infrastructure) |
| Round.lean | Rounding functions for ordered rings: `round`, `floor`, `ceil` with approximation properties and interaction with arithmetic operations |
| SuccPred.lean | Successor and predecessor functions in ordered algebraic contexts: compatibility with addition (`succ a = a + 1` in `SuccAddOrder`) and order preservation |
| ToIntervalMod.lean | Modular arithmetic mapping to intervals: `toIcoMod`, `toIocMod` reduce elements to canonical representatives in half-open intervals, essential for periodic functions and angle-like values |
| UpperLower.lean | Upper/lower sets in ordered algebraic structures: characterization via multiplicative/additive closure |
| Invertible.lean | Invertible elements in ordered structures: interaction of invertibility with order relations |
| AddGroupWithTop.lean | Additive groups with top element adjoined: extended arithmetic `a + ⊤ = ⊤` for non-archimedean constructions |
| AddTorsor.lean | Ordered additive torsors (affine spaces): affine combination respects order when acting on ordered types |
| Disjointed.lean | Disjointed sequences from monotone sequences: construction of pairwise disjoint sets from monotone families via `disjointed f n = f n \ f (n-1)` |
| PartialSups.lean | Partial suprema sequences: `partialSups f n = ⨆ i ≤ n, f i` with monotonicity and limit properties |
| Pi.lean | Ordered algebraic structures on Pi types (function spaces): componentwise order with algebraic operations |
| Sum.lean | Ordered algebraic structures on sum types: lexicographic and product orderings with algebraic compatibility |
| PUnit.lean | Ordered algebraic instances for the unit type `PUnit`: trivial implementations serving as base cases |

## Subdirectories

- [x] `Group/` - Comprehensive ordered group theory: bundled and unbundled definitions, absolute value (`|a|ₘ = max a a⁻¹`), Jordan decomposition (`a = a⁺ - a⁻`), positive cones, pointwise operations, group actions, sharp integer bounds exploiting distinctness, and lattice-ordered groups
- [x] `Monoid/` - Ordered monoid theory with bundled typeclasses (`IsOrderedMonoid`, `CanonicallyOrderedMul`) and unbundled framework (`CovariantClass`, `ContravariantClass`), covering products, units, type tags, WithTop/WithBot constructions, unique units theorem for canonical orderings, and locally finite characterizations
- [x] `Ring/` - Comprehensive ordered ring theory spanning unbundled foundations (minimal assumptions, rational ordering), classical algebraic ordering theory (preorderings, support ideals, Lam 1984), and bundled typeclasses with Bernoulli inequality, geometric series, archimedean classes, nonarchimedean functions, positive cones, and idempotent Boolean algebras
- [x] `Field/` - Ordered fields and division rings: unbundled framework with division inequalities, integer power parity-dependent signs, geometric series bounds, canonically ordered semifields, and subfield inheritance
- [x] `GroupWithZero/` - Comprehensive theory of ordered groups/monoids with zero for valuation theory: `LinearOrderedCommGroupWithZero` definitions, `WithZero` construction, lexicographic products, fine-grained unbundled typeclasses for multiplication monotonicity (`PosMulMono`, `MulPosMono`, etc.), order isomorphisms enabling lattice distribution, and transfer to order type synonyms
- [x] `Module/` - Ordered modules over ordered rings: fine-grained monotonicity typeclasses (`PosSMulMono`, `SMulPosMono`, etc.), bundled ordered module types (`IsOrderedModule`, `IsStrictOrderedModule`), **Hahn embedding theorem** (embedding linearly ordered modules into lexicographically ordered Hahn series), Archimedean module theory with class-based submodules, positive linear maps, and pointwise bounds on scalar multiplication
- [x] `Floor/` - Floor and ceiling functions: natural-valued (`FloorSemiring`, ⌊a⌋₊, ⌈a⌉₊) and integer-valued (`FloorRing`, ⌊a⌋, ⌈a⌉) with Galois connections `⌊a⌋₊ ≤ n ↔ a < n+1`, fractional parts (`fract a ∈ [0,1)`), division operators (⌊/⌋, ⌈/⌉), extended functions (ℝ≥0∞ → ℕ∞), and `positivity`/`norm_num` tactic extensions
- [x] `Archimedean/` - Archimedean ordered structures: core `Archimedean`/`MulArchimedean` typeclasses (∀x y>0, ∃n, x ≤ n•y), archimedean classes partitioning groups by "infinitesimal order", uniqueness of ordered ring homomorphisms to archimedean fields, indicator/cardinality results, and submonoid inheritance
- [x] `Hom/` - Order-preserving homomorphisms: bundled types for ordered monoid/ring homomorphisms and isomorphisms (`OrderMonoidHom`, `OrderRingHom`, `→*o`, `→+*o`), homomorphism classes for norms and seminorms (`GroupNormClass`, `RingSeminormClass`, `SubadditiveHomClass`, `SubmultiplicativeHomClass`), specialized results for submonoids, type tags, and units
- [x] `BigOperators/` - Order-theoretic properties of big operators (sums/products over finsets, lists, multisets): monotonicity lemmas, submultiplicativity/subadditivity, **Cauchy-Schwarz inequality** in multiple forms (standard, Sedrakyan's/Titu's/Engel's lemma), product/sum monotonicity under nonnegativity (`prod_le_prod`, `sum_le_sum`), and expectation operator properties
- [x] `Star/` - Star-ordered rings where order is characterized by star operation: `x ≤ y ↔ y = x + p` with `p ∈ closure{star s * s}`, generalizing C*-algebras, with self-adjoint element characterization, conjugation monotonicity (`star c * a * c`), star projections, and instances for product/Pi types
- [x] `Sub/` - Comprehensive theory of ordered subtraction via `OrderedSub` typeclass (`a - b ≤ c ↔ a ≤ c + b`), unifying normal subtraction in ordered groups and truncated subtraction (tsub) in canonically ordered monoids (ℕ, Multiset, ENNReal), with unbundled theory for fine-grained control via `AddLECancellable` and homomorphism preservation results
- [x] `Interval/` - Comprehensive interval arithmetic and operations: full-precision algebraic operations (addition, multiplication, powers, subtraction, division, negation) on abstract interval types (`NonemptyInterval α`, `Interval α`) with correctness proofs under monotonicity, and systematic development for finsets (`Finset.Ixx`), multisets (`Multiset.Ixx`), and sets (`Set.Ixx`) including translation operations, bijections, unit interval [0,1] algebraic instances, and successor-predecessor relations
- [x] `Nonneg/` - Comprehensive nonnegative subtype theory: core arithmetic instances (Zero, One, Add, Mul, Pow), bundled ordered ring structures (`IsOrderedRing`, `IsStrictOrderedRing`), semifield instances with units-positive equivalence (`unitsEquivPos`), module structures over nonnegative scalars, complete lattice instances (ConditionallyCompleteLinearOrderBot), and FloorSemiring support
- [x] `Positive/` - Algebraic structures for positive subtypes `{x : R // 0 < x}`: additive structures (semigroups with cancellation/monotonicity), multiplicative structures (monoids, ordered monoids, cancellative monoids), and for fields, commutative groups under multiplication with integer powers
- [x] `SuccPred/` - Specialized results for successor/predecessor in ordered algebraic structures: `SuccAddOrder` compatibility with partial suprema, type tags (`Multiplicative`/`Additive`) preserving successor structure, and `WithBot` algebraic successor properties (`succ (n : WithBot α) = n + 1`)
- [x] `AbsoluteValue/` - Core absolute value theory: bundled `AbsoluteValue R S` structure extending `MulHom` with nonnegativity/triangle inequality/positive definiteness, standard and trivial absolute values, nontriviality criteria, unbundled `IsAbsoluteValue` typeclass with bidirectional conversions, and Euclidean absolute values compatible with `EuclideanDomain` structure
- [x] `Antidiag/` - Antidiagonals in ordered contexts: finsets of tuples summing/multiplying to fixed values via `HasAntidiagonal` typeclass, with `piAntidiag` for functions (finset of functions summing to n), `finsuppAntidiag` for finitely supported functions, and `finMulAntidiag` for multiplicative antidiagonals with counting factorizations of squarefree integers (`#{d-tuples with product n} = d^(ω n)`)
- [x] `CauSeq/` - Core Cauchy sequence theory for ordered fields: concrete `IsCauSeq` predicate and `CauSeq` type with algebraic operations (ring/module/algebra instances), series convergence (geometric series, ratio test, Cauchy product), and **Cauchy completion construction** as quotient type `Cauchy abv := CauSeq / equiv` with field instances, serving as foundation for constructing ℝ and p-adic numbers
- [x] `WithTop/` - Conversion from `WithTop α` to base type via `untop₀` mapping `⊤` to zero (mirroring `ENat.toNat`), with comprehensive simplification lemmas for algebraic operations (addition, negation, multiplication), order relations, and max/min operations

## Search Tags

ordered-algebra ordered-groups ordered-rings ordered-monoids ordered-modules ordered-fields bundled-typeclasses unbundled-typeclasses covariant-class contravariant-class monotonicity kleene-algebra quantale idempotent-semiring complete-field floor-ceiling galois-connection successor-predecessor rearrangement-inequality chebyshev-inequality cauchy-schwarz-inequality bernoulli-inequality monovary antivary additive-torsor absolute-value archimedean hahn-embedding interval-arithmetic nonnegative positive star-algebra modular-arithmetic cauchy-sequences cauchy-completion geometric-series ratio-test jordan-decomposition positive-cone group-with-zero valuation-theory finset-operations big-operators expectation lattice-ordered-groups submultiplicative subadditive ordered-subtraction truncated-subtraction tsub antidiagonal euclidean-absolute-value ordered-homomorphisms order-isomorphisms with-top with-bot canonically-ordered divisibility-order partial-sups disjointed-sequences
