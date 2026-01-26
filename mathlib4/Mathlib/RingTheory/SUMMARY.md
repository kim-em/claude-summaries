---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory
generated: 2026-01-26T19:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 62
subdirs_count: 62
---

# RingTheory

## Overview

The `RingTheory/` directory contains comprehensive formalizations of commutative and non-commutative ring theory, including classical results and modern developments. This covers the fundamental theory of ideals, modules, and ring homomorphisms; structural classifications (integral domains, PIDs, UFDs, Dedekind domains); localization theory; completions (adic, Henselian); polynomial and power series rings (univariate, multivariate, Laurent, Hahn); algebraic constructions (adjoin root, tensor products, graded algebras); homological properties (flatness, projectivity, length, dimension); specialized structures (Witt vectors, divided powers, coalgebras); and important theorems (Nakayama's lemma, Hopkins-Levitzki, Nullstellensatz, Noether normalization).

## Key Files

| File | Purpose |
|------|---------|
| IntegralDomain.lean | Fundamental results on integral domains including finite domain-to-field theorem, cyclic unit groups, coprime factorization lemmas |
| PrincipalIdealDomain.lean | Principal ideal rings and domains; Bézout rings; proves PIDs are UFDs and Euclidean domains are PIDs |
| PrincipalIdealDomainOfPrime.lean | Criterion for when quotients of PIDs are PIDs using prime ideal theory |
| AdjoinRoot.lean | Construction of R[X]/(f) for adjoining roots of polynomials; lift homomorphisms, equivalences, field structure for irreducible polynomials |
| IsAdjoinRoot.lean | Generalized interface for all R[α] constructions independent of specific implementation |
| Multiplicity.lean | Theory of multiplicity of divisors in commutative monoids; finite/infinite multiplicity, valuations |
| Nakayama.lean | Nakayama's lemma and variants from Stacks Project including Jacobson ideal versions |
| LaurentSeries.lean | Formal Laurent series R⸨X⸩ as HahnSeries ℤ; Hasse derivatives, X-adic valuation, embedding from power series and rational functions |
| PowerBasis.lean | Power basis structure giving R-algebra basis as {1, x, x², ..., xⁿ}; used for algebraic extensions |
| Henselian.lean | Henselian rings and local rings; lifting simple roots from quotients, adic completeness implies Henselian |
| Binomial.lean | Binomial rings with generalized binomial coefficients (multichoose/choose), Chu-Vandermonde identity |
| ChainOfDivisors.lean | Chains of divisors and associated well-foundedness properties |
| ClassGroup.lean | Class group of a Dedekind domain as quotient of fractional ideals by principal ideals |
| Complex.lean | Ring structure on complex numbers (likely re-exports) |
| Conductor.lean | Conductor ideal theory for ring extensions |
| Discriminant.lean | Discriminant of algebraic elements and bases |
| DualNumber.lean | Dual numbers R[ε]/(ε²) construction |
| EssentialFiniteness.lean | Essential finiteness conditions for ring homomorphisms (finite generation modulo nilradical) |
| EuclideanDomain.lean | Euclidean domain basics and relationship to principal ideal domains |
| Filtration.lean | Filtered rings and modules (I-filtrations, stable/antitone/separated filtrations) |
| FiniteLength.lean | Modules of finite length (composition series) |
| FinitePresentation.lean | Finitely presented algebras and modules |
| FiniteStability.lean | Stability of finiteness properties under base change |
| FiniteType.lean | Finitely generated algebras (finite type over base ring) |
| Fintype.lean | Finite rings as fintypes |
| FreeCommRing.lean | Free commutative ring construction R[α] as polynomial ring with noncommutative multiplication allowed |
| FreeRing.lean | Free (non-commutative) ring construction |
| Frobenius.lean | Frobenius endomorphism in characteristic p; perfect rings |
| Grassmannian.lean | Grassmannian scheme construction |
| HopkinsLevitzki.lean | Hopkins-Levitzki theorem: Artinian implies Noetherian for rings satisfying ACC on annihilators |
| Idempotents.lean | Theory of idempotent elements; orthogonal idempotents, lifting idempotents through surjections |
| IsPrimary.lean | Primary ideals (powers of primes divide into ideal implies prime or power in ideal) |
| IsTensorProduct.lean | Universal property characterization of tensor products |
| Lasker.lean | Lasker rings (Noetherian rings where every ideal has primary decomposition) |
| Length.lean | Length of modules (supremum of composition series lengths) |
| LinearDisjoint.lean | Linear disjointness of field extensions and subalgebras |
| LittleWedderburn.lean | Wedderburn's little theorem: finite division rings are fields |
| MatrixAlgebra.lean | Matrix algebras over commutative rings |
| MatrixPolynomialAlgebra.lean | Polynomial rings over matrix algebras |
| MvPolynomial.lean | Multivariate polynomial ring imports (main content in MvPolynomial/ subdirectory) |
| NoetherNormalization.lean | Noether normalization lemma for finitely generated algebras over fields |
| NormTrace.lean | Norm and trace functions for ring extensions (likely imports) |
| NormalClosure.lean | Normal closure of ring extensions |
| Nullstellensatz.lean | Hilbert's Nullstellensatz (weak and strong forms) |
| OrderOfVanishing.lean | Order of vanishing for functions at points (multiplicity in local rings) |
| OrzechProperty.lean | Orzech property for Prüfer domains |
| Perfection.lean | Perfection of rings in characteristic p (inverse limit under Frobenius) |
| PiTensorProduct.lean | Tensor products of families of modules indexed by types |
| PicardGroup.lean | Picard group of invertible modules (line bundles); Pic(R) as abelian group |
| PolynomialAlgebra.lean | Polynomial algebras and their properties |
| Prime.lean | Prime elements in rings and their basic properties |
| QuotSMulTop.lean | Quotients by scalar multiplication in modules |
| Radical.lean | Radical of ideals (nilradical, Jacobson radical) |
| ReesAlgebra.lean | Rees algebra of an ideal (graded algebra construction) |
| RingHomProperties.lean | Properties preserved by ring homomorphisms |
| RingInvo.lean | Ring involutions (anti-automorphisms of order 2) |
| Support.lean | Support of module elements and functions |
| SurjectiveOnStalks.lean | Ring homomorphisms surjective on stalks (for sheaf theory) |
| ZMod.lean | Integers modulo n (likely imports from ZMod/ subdirectory) |
| ZariskisMainTheorem.lean | Zariski's main theorem on quasi-finite morphisms |
| AlgebraTower.lean | Tower laws for algebras (transitivity of algebraic properties) |
| Bezout.lean | Bézout domains (finitely generated ideals are principal) |

## Subdirectories

- [x] `AdicCompletion/` - Adic completions of rings with respect to ideals
- [x] `Adjoin/` - Theory of adjoining elements to rings and algebras
- [x] `Algebraic/` - Algebraic elements and algebraic extensions of rings
- [x] `AlgebraicIndependent/` - Algebraically independent sets and transcendence bases
- [x] `Artinian/` - Artinian rings and modules (descending chain condition)
- [x] `Bialgebra/` - Bialgebras (algebras with compatible coalgebra structure)
- [x] `Coalgebra/` - Coalgebras (dual notion to algebras)
- [x] `Congruence/` - Congruence relations on rings
- [x] `Coprime/` - Coprime ideals and elements
- [x] `DedekindDomain/` - Dedekind domains (Noetherian integrally closed dimension 1 domains)
- [x] `Derivation/` - Derivations on rings and modules (Leibniz rule operators)
- [x] `DiscreteValuationRing/` - Discrete valuation rings (DVRs)
- [x] `DividedPowers/` - Divided power structures on ideals
- [x] `Etale/` - Étale algebras and morphisms
- [x] `Extension/` - Ring extensions and their properties
- [x] `FilteredAlgebra/` - Filtered algebras and associated graded algebras
- [x] `Finiteness/` - Various finiteness conditions (finite type, finite presentation, etc.)
- [ ] `Flat/` - Flat modules and algebras
- [ ] `FractionalIdeal/` - Fractional ideals over Dedekind domains
- [ ] `GradedAlgebra/` - Graded rings and algebras
- [ ] `HahnSeries/` - Hahn series (generalization of Laurent series)
- [ ] `HopfAlgebra/` - Hopf algebras (bialgebras with antipode)
- [ ] `Ideal/` - Comprehensive ideal theory (operations, quotients, primes, maximals)
- [ ] `IdealFilter/` - Filters of ideals
- [ ] `Int/` - Ring-theoretic properties specific to integers
- [ ] `IntegralClosure/` - Integral closure of rings in extensions
- [ ] `Invariant/` - Invariant theory (invariants under group actions)
- [ ] `Jacobson/` - Jacobson rings and radical theory
- [ ] `Kaehler/` - Kähler differentials for ring homomorphisms
- [ ] `KrullDimension/` - Krull dimension of rings and modules
- [ ] `LocalProperties/` - Properties of ring homomorphisms that can be checked locally
- [ ] `LocalRing/` - Local rings (unique maximal ideal) and their properties
- [ ] `Localization/` - Localization of rings at multiplicative sets
- [ ] `Morita/` - Morita equivalence of rings and modules
- [ ] `MvPolynomial/` - Multivariate polynomials in detail
- [ ] `MvPowerSeries/` - Multivariate formal power series
- [ ] `Nilpotent/` - Nilpotent elements and nilradical
- [ ] `Noetherian/` - Noetherian rings and modules (ascending chain condition)
- [ ] `NonUnitalSubring/` - Non-unital subrings (rngs)
- [ ] `NonUnitalSubsemiring/` - Non-unital subsemirings
- [ ] `Norm/` - Norm maps for ring extensions
- [ ] `OreLocalization/` - Ore localization for non-commutative rings
- [ ] `Perfectoid/` - Perfectoid rings (adic spaces in arithmetic geometry)
- [ ] `Polynomial/` - Univariate polynomial theory in detail
- [ ] `PolynomialLaw/` - Polynomial laws and functions
- [ ] `PowerSeries/` - Formal power series R⟦X⟧
- [ ] `QuasiFinite/` - Quasi-finite algebras and morphisms
- [ ] `Regular/` - Regular rings and regular sequences
- [ ] `RingHom/` - Ring homomorphism theory and properties
- [ ] `RootsOfUnity/` - Roots of unity in rings
- [ ] `SimpleModule/` - Simple modules (no nontrivial submodules)
- [ ] `SimpleRing/` - Simple rings (no nontrivial two-sided ideals)
- [ ] `Smooth/` - Smooth algebras and morphisms
- [ ] `Spectrum/` - Prime spectrum of rings (Spec R)
- [ ] `TensorProduct/` - Tensor products of algebras and modules
- [ ] `Trace/` - Trace maps for ring extensions
- [ ] `TwoSidedIdeal/` - Two-sided ideals in non-commutative rings
- [ ] `UniqueFactorizationDomain/` - Unique factorization domains (UFDs)
- [ ] `Unramified/` - Unramified extensions and morphisms
- [ ] `Valuation/` - Valuations on rings and fields
- [ ] `WittVector/` - Witt vectors (p-adic algebraic constructions)
- [ ] `ZMod/` - Ring structure on ℤ/nℤ

## Search Tags

ring-theory commutative-algebra ideal principal-ideal-domain PID unique-factorization-domain UFD Dedekind-domain localization completion adic Henselian polynomial power-series Laurent-series multivariate Noetherian Artinian module homological-algebra tensor-product flatness integral-closure algebraic-extension Galois valuation discrete-valuation-ring spectrum prime-ideal maximal-ideal Nakayama binomial Frobenius characteristic-p Witt-vector graded-algebra filtered-algebra Kaehler-differential dimension Krull-dimension local-ring residue-field quotient AdjoinRoot nullstellensatz Noether-normalization Hopkins-Levitzki multiplicity class-group Picard-group etale smooth unramified perfectoid
