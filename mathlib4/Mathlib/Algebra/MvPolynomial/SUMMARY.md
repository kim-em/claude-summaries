---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/MvPolynomial
generated: 2025-12-01T20:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 21
subdirs_count: 0
---

# MvPolynomial

## Overview

The `MvPolynomial/` directory implements multivariate polynomial theory for polynomial rings `MvPolynomial σ R`, representing `R[X_i : i ∈ σ]` where `σ` is an arbitrary (potentially infinite) type indexing the variables and `R` is a commutative semiring. Built on `AddMonoidAlgebra R (σ →₀ ℕ)`, it provides comprehensive machinery including evaluation and renaming operations, degree theory with `degrees`, `degreeOf`, and `totalDegree`, equivalences between polynomial rings, monadic operations `bind₁`/`join₁` and `bind₂`/`join₂`, derivations and partial derivatives `pderiv`, division by monomials, variable analysis, and algorithmic results including the Schwartz-Zippel lemma for probabilistic polynomial identity testing.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `MvPolynomial σ R` type as `AddMonoidAlgebra R (σ →₀ ℕ)`, monomials `monomial s a`, constants `C a`, variables `X i`, coefficients `coeff s p`, commutative semiring structure, algebra instances, and foundational lemmas |
| Eval.lean | Evaluation functions: `eval₂` (evaluate with coefficient map and variable valuation), `eval` (direct evaluation), `map` (coefficient semiring homomorphism), `aeval` (algebraic evaluation), and their algebraic properties |
| Degrees.lean | Degree theory: `degrees p` (multiset of variables with multiplicities), `degreeOf n p` (degree in variable `n`), `totalDegree p` (maximum total degree of monomials), and degree bounds for polynomial operations |
| Variables.lean | Variable set analysis: `vars p` (finset of variables appearing in `p`), relationships between variables and polynomial operations, support properties |
| Rename.lean | Variable renaming: `rename f` (apply function `f : σ → τ` to variable indices), `renameEquiv` (equivalence induced by bijection), interaction with evaluation and other operations |
| Equiv.lean | Polynomial ring equivalences: `pUnitAlgEquiv` (single variable ≃ univariate polynomials `R[X]`), equivalences induced by variable type equivalences, `finSuccEquiv` (Fin (n+1) ≃ Option (Fin n)), isomorphisms between polynomial rings |
| Monad.lean | Monadic operations: `bind₁` and `join₁` (operate on variable type `σ`, make polynomial ring a monad), `bind₂` and `join₂` (operate on coefficient type `R`, ring homomorphisms), interactions with `rename` and `map` |
| Derivation.lean | Derivation theory: `mkDerivationₗ` and `mkDerivation` (construct derivations from values on variables), `mkDerivationEquiv` (linear equivalence between `σ → A` and derivations), universal properties |
| PDeriv.lean | Partial derivatives: `pderiv i p` (formal partial derivative with respect to variable `i`), derivation properties, Leibniz rule, interaction with evaluation and degrees |
| CommRing.lean | Commutative ring structure for `MvPolynomial σ R` when `R` is a `CommRing`, stronger results available with ring rather than semiring coefficients |
| Division.lean | Monomial division: `divMonomial p s` (divide by monomial with exponents `s`, discarding non-divisible terms), `modMonomial p s` (remainder), division algorithm properties |
| Comap.lean | Comap operation: mapping polynomials backward along algebra homomorphisms, adjointness properties with evaluation |
| Counit.lean | Counit map: the algebra homomorphism from `MvPolynomial σ R` to `R` sending all variables to zero, categorical properties |
| Expand.lean | Expansion operation: `expand p` (raise all variable exponents by factor `p`, so `∑ aₙ xⁿ` becomes `∑ aₙ xⁿᵖ`), algebra homomorphism properties |
| Funext.lean | Function extensionality for polynomials: when two polynomials are equal if they evaluate to the same values |
| Supported.lean | Support restrictions: polynomials supported on a subset of variables, characterizing when variables don't appear |
| Nilpotent.lean | Nilpotent elements: theory of polynomials that become zero when raised to some power |
| Invertible.lean | Invertible elements: characterization of units in multivariate polynomial rings |
| Cardinal.lean | Cardinality bounds: relating cardinalities of coefficient rings, variable sets, and polynomial rings |
| Polynomial.lean | Connection to univariate polynomials: relating `MvPolynomial σ R` to `Polynomial R` in special cases |
| SchwartzZippel.lean | Schwartz-Zippel lemma: probabilistic bounds on zeros of nonzero polynomials, proves `schwartz_zippel_sup_sum`, `schwartz_zippel_sum_degreeOf`, `schwartz_zippel_totalDegree` for polynomial identity testing over integral domains |

## Subdirectories

(none)

## Search Tags

multivariate-polynomial polynomial evaluation degree total-degree partial-derivative derivation monomial division rename equivalence monad bind join expand schwartz-zippel polynomial-identity-testing variables coefficient commutative-algebra formal-derivative
