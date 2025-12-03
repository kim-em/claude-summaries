---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/BigOperators
generated: 2025-12-01T19:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 15
subdirs_count: 4
---

# BigOperators

## Overview

The `BigOperators/` directory provides the complete infrastructure for finite sums (`∑`) and products (`∏`) across all algebraic structures in mathlib4. At its core is a carefully stratified three-layer hierarchy (List → Multiset → Finset) implemented in the `Group/` subdirectory, which establishes the foundational big operator definitions for commutative monoids. This hierarchical design reflects fundamental mathematical principles: `List.prod` operates on ordered sequences via `foldr`, `Multiset.prod` quotients out permutations while preserving multiplicity, and `Finset.prod` provides the user-facing notation `∏ i ∈ s, f i` for finite sets. Building on this foundation, the directory extends big operators to richer structures: `Ring/` adds interaction between additive and multiplicative operations (distributivity, products-of-sums, binomial formulas), `GroupWithZero/` handles zero-propagation and scalar actions, and `Finsupp/` provides specialized operations for finitely-supported functions. Beyond the core hierarchical infrastructure, the directory includes 15 specialized files covering variant notations (finprod/finsum for finite support without `Fintype` constraints, expectations `𝔼` for averages), operations on specific types (Fin, Option, Pi types, intervals, antidiagonals), and theoretical connections to modular arithmetic, associated/prime elements, ring equivalences, summation by parts, balancing functions, and extensions to structures with top/bottom elements.

## Key Files

| File | Purpose |
|------|---------|
| Associated.lean | Products of associated, prime, and irreducible elements: theorems connecting `Algebra.Associated` definitions with products over multisets, finsets, and finsupps, including `Prime.exists_mem_multiset_dvd` |
| Balance.lean | Function balancing (function minus its average): defines `Fintype.balance f = f - 𝔼 y, f y`, the unique function with same pairwise differences as `f` but summing to zero, useful for Fourier analysis |
| Expect.lean | Average/expectation over finsets: defines `Finset.expect` with notation `𝔼 i ∈ s, f i` for uniform-weighted expectations, a special case of convex combinations with extensive API for algebraic manipulation |
| Field.lean | Big operators in division semirings/fields: results about sums and products with division, including `Finset.sum_div` and density operations for finsets |
| Fin.lean | Big operators over `Fin` type: induction formulas `Fin.prod_univ_castSucc` and `Fin.prod_univ_succ`, product of constant functions, and `finFunctionFinEquiv` (equivalence between `Fin n → Fin m` and `Fin (m ^ n)`) |
| Finprod.lean | Finite products/sums over types without finiteness hypotheses: `finprod`/`finsum` (notation `∏ᶠ`/`∑ᶠ`) produce junk values (1/0) for infinite supports, easier than `Finset.sum` when avoiding `Fintype` data |
| Intervals.lean | Big operators over intervals: results for products/sums over `Ico`, `Ioc`, and other interval types with shifting and subtraction operations, includes factorial-related lemmas |
| ModEq.lean | Modular congruence preservation: proves `f i ≡ g i [MOD n]` for all `i ∈ s` implies `∏ i ∈ s, f i ≡ ∏ i ∈ s, g i [MOD n]` for lists, multisets, and finsets with both natural and integer modular arithmetic |
| Module.lean | Summation by parts (Abel's lemma): defines `sum_Ico_by_parts` and `sum_range_by_parts` formulas for transforming sums of products `∑ f i • g i` using partial sums |
| NatAntidiagonal.lean | Big operators over natural antidiagonals: theorems for `Finset.Nat.antidiagonal` including `prod_antidiagonal_succ`, swap operations, and substitution formulas |
| Option.lean | Products/sums over `Option α`: formulas for `Finset.insertNone` and `Finset.eraseNone` relating optional elements to base finset operations |
| Pi.lean | Big operators for Pi types (dependent products): theorems about products/sums of functions returning elements of monoid-valued type families, including `Finset.prod_apply` |
| RingEquiv.lean | Ring equivalences preserve big operators: `RingEquiv.map_prod` and `RingEquiv.map_sum` showing ring isomorphisms commute with products/sums, including opposite ring operations |
| Sym.lean | Big operators involving symmetric powers: lemmas on `Finset.sum` and `Finset.prod` for `Finset.sym2` (unordered pairs) and `Finset.sym` (symmetric powers), including off-diagonal sums |
| WithTop.lean | Sums/products in `WithTop`/`WithBot`: characterizes when sums/products are infinite (⊤/⊥) in monoids extended with top/bottom elements, finiteness conditions for products of nonzero elements |

## Subdirectories

- [x] `Group/` - Foundational three-layer hierarchy (List → Multiset → Finset) for big operators over commutative monoids: `List` layer defines ordered products/sums via `foldr`, `Multiset` layer quotients by permutation equivalence with invariance proofs, `Finset` layer provides user-facing notation `∏ i ∈ s, f i` and `∑ i ∈ s, f i` with comprehensive theory including homomorphisms, alternating products, powersets, sigma types, Pi types, intervals, indicators, and piecewise functions (3 subdirectories, 15 total files)
- [x] `Ring/` - Big operators for ring structures extending the group hierarchy: implements interaction between additive and multiplicative operations including distributivity (`mul_sum`, `sum_mul`), products-of-sums via powersets (`prod_add`, `prod_sum`), zero-propagation, binomial-style formulas, commutativity preservation, divisibility lemmas, natural/integer coercion preservation, and specialized parity analysis for natural numbers (4 files: List, Multiset, Finset, Nat)
- [x] `GroupWithZero/` - Big operators for structures with zero elements: zero-propagation theorems (`prod_eq_zero`, `prod_eq_zero_iff` requiring no zero divisors), support characterization via `support_prod`, conditional products with indicators (`prod_ite_zero`, `prod_boole`), units construction (`Units.mk0_prod`), and scalar action distributivity over sums/products for three variants (`DistribSMul`, `MulDistribMulAction`, `SMulCommClass`) with permutation invariance (2 files: Finset, Action)
- [x] `Finsupp/` - Big operators for finitely-supported functions: defines `Finsupp.sum` and `Finsupp.prod` iterating over support sets, extensive API for index transformations (`prod_add_index`, `prod_mapRange_index`), homomorphism properties (`map_finsuppProd`), canonical isomorphism `liftAddHom : (α → M →+ N) ≃+ ((α →₀ M) →+ N)`, specialized results for `Fin` decompositions (`sum_cons`, `finTwoArrowEquiv'`), and connections to indicator functions and domain embeddings (2 files: Basic, Fin)

## Search Tags

big-operators finset multiset list sum product finprod finsum hierarchy three-layer list-prod multiset-prod finset-prod foldr quotient permutation-invariance commutative-monoid alternating-product telescoping expectation average balance summation-by-parts abel-lemma fin intervals natural-antidiagonal modular-arithmetic nat-modeq int-modeq associated-elements prime-elements irreducible-elements ring-equivalence ring-homomorphism pi-types option symmetric-powers sym2 with-top with-bot field division distribsmul muldistribmulaction smulcommclass scalar-action group-with-zero monoid-with-zero zero-propagation prod-eq-zero zero-divisors support units distributivity mul-sum sum-mul prod-add prod-sum powerset binomial commutativity divisibility parity coercion finsupp finitely-supported-functions liftAddHom index-transformation indicator piecewise preimage sigma-type homomorphism ordered-sequences unordered-collections indexed-operators mathlib4-foundations
