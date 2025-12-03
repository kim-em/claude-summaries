---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Polynomial
generated: 2025-12-01T19:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 41
subdirs_count: 3
---

# Polynomial

## Overview

The `Polynomial/` directory provides the complete mathematical theory of univariate polynomials `R[X]` in Lean 4's mathlib. Built on `AddMonoidAlgebra R ℕ`, it establishes polynomials as a fundamental algebraic structure with rich theory spanning 41 files and 3 specialized subdirectories. The implementation covers the full spectrum from foundational definitions (monomials, constant embedding `C`, variable `X`, coefficient access) through algebraic operations (semiring/ring/algebra instances, evaluation homomorphisms, composition, mapping) to sophisticated mathematical theory including degree calculus, formal derivatives, division algorithms, root theory with multiplicities, factorization, splitting fields, and specialized constructions like Laurent polynomials and partial fractions.

The three subdirectories provide deep theory for core polynomial operations: `Degree/` develops comprehensive degree theory with leading/trailing coefficients and domain properties; `Eval/` establishes evaluation as ring homomorphisms with irreducibility preservation; and `Module/` constructs polynomial module structures connecting polynomials with module theory through evaluation actions and tensor products. Together with the top-level files covering derivatives (formal and Hasse), division (Euclidean domain structure, root multiplicities), roots and factorization (multisets with multiplicities, splitting predicates), and advanced topics (Taylor expansion, Descartes' rule of signs, homogenization), this directory forms mathlib's foundational polynomial library used throughout algebraic and analytic mathematics.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `Polynomial R` structure wrapping `AddMonoidAlgebra R ℕ`, `monomial n a` (polynomial `a X^n`), `C a` (constant polynomial), `X` (the variable), semiring structure, coefficient operations, and fundamental API |
| AlgebraMap.lean | Algebra structure on `A[X]` when `A` is an `R`-algebra, `aeval` (algebra homomorphism from `R[X]` to `A` given valuation), and `mapAlgHom` for applying algebra homomorphisms to coefficients |
| Coeff.lean | Theory of polynomial coefficients: accessing, manipulating, and relating coefficients to polynomial structure |
| CoeffList.lean | Converting polynomials to/from coefficient lists |
| CoeffMem.lean | Membership properties for coefficients |
| Monomial.lean | Theory of monomial polynomials |
| Basis.lean | Polynomial basis theory |
| BigOperators.lean | Interaction of polynomials with big sums and products (14KB of lemmas) |
| Derivative.lean | Formal derivative as linear map `derivative : R[X] →ₗ[R] R[X]`, iterated derivatives via `derivativeFinsupp` |
| HasseDeriv.lean | Hasse derivatives (normalized higher derivatives for characteristic p) |
| SumIteratedDerivative.lean | Sums of iterated derivatives |
| Monic.lean | Monic polynomials (leading coefficient 1): closure properties, constructions, and fundamental lemmas |
| Div.lean | Division of univariate polynomials: `divByMonic`, `modByMonic`, compatibility via `modByMonic_add_div`, and `rootMultiplicity` |
| RingDivision.lean | Division theory in rings |
| FieldDivision.lean | Division and root multiplicity theory in fields, euclidean domain structure, unique factorization |
| Roots.lean | Multiset of roots `roots p` with multiplicities, distinct root set `rootSet p E` in algebra `E`, factorization as `C leadingCoeff * ∏ (X - a)` |
| Factors.lean | Polynomial factorization theory |
| Splits.lean | Split polynomials: predicate `Splits i f` meaning polynomial `f` factors completely over field extension via `i : K →+* L` |
| Reverse.lean | Polynomial reversal: reversing coefficient order |
| Mirror.lean | Mirror operation on polynomials |
| EraseLead.lean | Erasing leading terms from polynomials |
| Expand.lean | Polynomial expansion operations |
| Taylor.lean | Taylor expansion of polynomials |
| Inductions.lean | Induction principles for polynomials |
| Identities.lean | Polynomial identities |
| Laurent.lean | Laurent polynomials `R[T;T⁻¹]` allowing negative exponents, defined as `AddMonoidAlgebra R ℤ`, with constant inclusion `C` and variable powers `T` |
| Bivariate.lean | Theory of polynomials in two variables |
| UnitTrinomial.lean | Unit trinomials (trinomials with unit coefficients) |
| CancelLeads.lean | Leading term cancellation |
| Cardinal.lean | Cardinality properties of polynomials |
| DenomsClearable.lean | Denominators clearable from polynomial expressions |
| Derivation.lean | Polynomial derivations |
| GroupRingAction.lean | Group and ring actions on polynomials |
| Homogenize.lean | Homogenization of polynomials |
| Lifts.lean | Lifting polynomials along ring homomorphisms |
| OfFn.lean | Constructing polynomials from functions |
| PartialFractions.lean | Partial fraction decomposition |
| RuleOfSigns.lean | Descartes' rule of signs: `signVariations` counts sign changes in coefficients, theorem proving positive roots (with multiplicity) ≤ sign changes |
| Sequence.lean | Polynomial sequences |
| Smeval.lean | Scalar multiplication evaluation |
| SpecificDegree.lean | Theory of polynomials of specific degree |

## Subdirectories

- [x] `Degree/` - Comprehensive degree theory (11 files): core definitions (`degree`, `natDegree`, `leadingCoeff`, `Monic`), extensive operation lemmas, trailing degree theory (`trailingDegree`, `natTrailingDegree`, `trailingCoeff`), domain properties for exact degree formulas, unit characterizations, small degree results, support relationships, and finite field absolute values
- [x] `Eval/` - Polynomial evaluation theory (7 files): core evaluation operations (`eval₂`, `eval`, `comp`, `map`) as ring homomorphisms, interactions with degrees and coefficients, algebra homomorphism properties, irreducibility preservation under mapping (crucial for reduction modulo primes), scalar multiplication interactions, and subring characterizations
- [x] `Module/` - Polynomial module structures (4 files): `Module.AEval R M a` constructing `R[X]`-modules via evaluation at algebra elements with invariant submodule theory, `PolynomialModule R M` as the polynomial module `M[X]` with evaluation/composition operations, torsion theory for finite-dimensional modules, and tensor product isomorphisms `R[X] ⊗[R] M ≃ M[X]`

## Search Tags

polynomial univariate semiring ring algebra coefficients monomial degree derivative roots monic division euclidean-domain factorization splitting evaluation aeval laurent-polynomial descartes-rule-of-signs taylor-expansion field-division root-multiplicity formal-derivative hasse-derivative
