---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory
generated: 2026-01-25T05:20:30Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 47
subdirs_count: 21
---

# NumberTheory

## Overview

The `NumberTheory/` directory provides a comprehensive formalization spanning the entire landscape of number theory, from elementary results to deep modern theorems. At the elementary level, it establishes foundational theory: primality testing (Lucas-Lehmer for Mersenne primes, Fermat pseudoprimes), divisibility and perfect numbers, factorization properties, Bertrand's postulate, Chebyshev's theorem, Wilson's theorem, and smooth numbers. Classical Diophantine theory includes complete solutions to Pell's equation, Pythagorean triples, sums of squares (Fermat's two-square theorem, Lagrange's four-square theorem), Matiyasevic's theorem on Diophantine sets, and verified proofs of Fermat's Last Theorem for n=3 and n=4.

The arithmetic function framework (`ArithmeticFunction/`) establishes the Dirichlet ring structure with Möbius inversion, von Mangoldt function, divisor sums, and multiplicative characters. This infrastructure supports advanced analytic number theory through the `LSeries/` subdirectory, which provides a complete treatment of L-series theory: Riemann and Hurwitz zeta functions with analytic continuation and functional equations, Dirichlet L-functions with Euler products and non-vanishing results, culminating in a full proof of Dirichlet's theorem on primes in arithmetic progressions.

Algebraic number theory is formalized through multiple interconnected subdirectories. The `NumberField/` framework defines number fields as finite extensions of ℚ with complete infrastructure: rings of integers as Dedekind domains with integral bases, fractional ideals, discriminants (Hermite-Minkowski theorem), class numbers and Minkowski bounds, infinite places (real/complex embeddings) and finite places (v-adic valuations), canonical embedding into ℝ^r₁ × ℂ^r₂ enabling geometric methods, adele rings for global-local perspectives, and Dirichlet's Unit Theorem. Specialized number field classes include `Cyclotomic/` (cyclotomic extensions ℚ(ζₙ) with Galois groups (ℤ/nℤ)ˣ, discriminant formulas, cyclotomic characters), `ClassNumber/` (finiteness via admissible absolute values for both number fields and function fields), and `Zsqrtd/` (quadratic integer rings ℤ[√d] with Gaussian integers ℤ[i] as a Euclidean domain).

The `Padics/` subdirectory develops p-adic number theory from valuations (Legendre's and Kummer's theorems) through construction of ℚ_p and ℤ_p with their complete nonarchimedean structures, Hensel's lemma, Mahler's theorem connecting continuous functions to vanishing sequences, and p-adic complex numbers ℂ_p. Local field theory (`LocalField/`) establishes general non-archimedean local fields with DVR structure and finite residue fields.

Additional specialized topics include `ModularForms/` (slash actions, Eisenstein series, Jacobi theta functions, Dedekind eta, q-expansions, Petersson product, Hecke bounds), `LegendreSymbol/` (quadratic reciprocity with Gauss and Eisenstein lemmas, Jacobi symbols, additive characters), `DirichletCharacter/` (primitive characters, conductors, Gauss sums, orthogonality), `DiophantineApproximation/` (Dirichlet's theorem, Legendre's theorem on continued fractions), `Harmonic/` (harmonic numbers with Euler-Mascheroni constant γ and connections to Γ'(n+1) and ζ(s) near s=1), `Height/` (height functions for Diophantine geometry), `RamificationInertia/` (ramification index and inertia degree in Galois extensions), and `Transcendental/` (Lindemann-Weierstrass analytic methods and Liouville's constructive transcendence via Diophantine approximation).

The directory seamlessly integrates computational tools (primality tests, factorization, norm bounds) with deep theoretical frameworks (class field theory infrastructure, analytic continuation, functional equations), providing a unified foundation for both elementary and advanced number-theoretic research in Lean.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core lemma for Witt vector construction: `dvd_sub_pow_of_dvd_sub` proving divisibility of power differences |
| Bertrand.lean | Proof of Bertrand's postulate: between any positive number and its double there exists a prime, using binomial coefficient bounds |
| LucasLehmer.lean | Lucas-Lehmer primality test for Mersenne numbers `2^p - 1` with certified computation via norm_num extension |
| Pell.lean | Complete theory of Pell's equation `x^2 - d*y^2 = 1` including existence of nontrivial solutions and fundamental solution characterization |
| PellMatiyasevic.lean | Pell equation solutions for the special case `d = a^2 - 1`, used in proving Matiyasevic's theorem |
| Dioph.lean | Diophantine sets and functions, Matiyasevic's theorem on the power function being Diophantine, connection to Hilbert's tenth problem |
| Divisors.lean | Divisor finsets, perfect numbers, antidiagonal pairs, sum/product operations over divisors |
| Multiplicity.lean | p-adic valuation and multiplicity theory for various ring structures |
| ArithmeticFunction.lean | Deprecated module redirecting to modular arithmetic function theory (Möbius, von Mangoldt, zeta) |
| Chebyshev.lean | Chebyshev's theorem and prime counting functions |
| SmoothNumbers.lean | Theory of smooth numbers (numbers with only small prime factors) |
| Divisors.lean | Comprehensive theory of divisor finsets including perfect numbers and antidiagonal products |
| Fermat.lean | Fermat's theorem on sums of two squares and related results |
| FermatPsp.lean | Fermat pseudoprimes and primality testing |
| SumTwoSquares.lean | Complete characterization of integers representable as sums of two squares |
| SumFourSquares.lean | Lagrange's four-square theorem: every natural number is a sum of four squares |
| PythagoreanTriples.lean | Classification and properties of Pythagorean triples |
| GaussSum.lean | Gauss sums and their properties in number theory |
| Wilson.lean | Wilson's theorem: (p-1)! ≡ -1 (mod p) for prime p |
| Primorial.lean | Primorials (product of first n primes) and their properties |
| PrimeCounting.lean | Prime counting function π(x) and related bounds |
| ZetaValues.lean | Special values of the Riemann zeta function |
| Bernoulli.lean | Bernoulli numbers and their number-theoretic properties |
| BernoulliPolynomials.lean | Bernoulli polynomials and their applications |
| KummerDedekind.lean | Kummer-Dedekind theorem for factorization of primes in field extensions |
| Modular.lean | Basic modular arithmetic and congruence theory |
| FrobeniusNumber.lean | Frobenius coin problem (largest number not representable as linear combination) |
| EllipticDivisibilitySequence.lean | Divisibility sequences arising from elliptic curves |
| MaricaSchoenheim.lean | Marica-Schoenheim inequality in combinatorial number theory |
| WellApproximable.lean | Well-approximable numbers and Diophantine approximation theory |
| SiegelsLemma.lean | Siegel's lemma on simultaneous Diophantine approximation |
| Ostrowski.lean | Ostrowski's theorem classifying absolute values on ℚ |
| ADEInequality.lean | ADE inequalities related to Dynkin diagrams and representation theory |
| AbelSummation.lean | Abel summation formula for transforming sums |
| Niven.lean | Niven's theorem on rational values of trigonometric functions |
| Rayleigh.lean | Rayleigh quotient and related number-theoretic applications |
| SelbergSieve.lean | Selberg sieve method for prime number theory |
| MahlerMeasure.lean | Mahler measure of polynomials |
| FactorisationProperties.lean | General factorization properties in rings |
| FunctionField.lean | Function fields and their number-theoretic properties |
| PowModTotient.lean | Powers modulo totient function |
| PrimesCongruentOne.lean | Dirichlet's theorem on primes in arithmetic progressions (mod 4) |
| LucasPrimality.lean | Lucas primality test |
| SelbergSieve.lean | Selberg sieve for bounding prime-related sums |
| SumPrimeReciprocals.lean | Divergence of sum of reciprocals of primes |
| TsumDivisorsAntidiagonal.lean | Infinite sums over divisor antidiagonals |
| TsumDivsorsAntidiagonal.lean | Typo variant redirecting to correct file |
| VonMangoldt.lean | Von Mangoldt function definition (import only) |

## Subdirectories

- [x] `ArithmeticFunction/` - Arithmetic functions (Möbius, von Mangoldt, Dirichlet convolution, multiplicative functions)
- [x] `ClassNumber/` - Class number theory for number fields and quadratic forms
- [x] `Cyclotomic/` - Cyclotomic fields and polynomials
- [x] `DiophantineApproximation/` - Diophantine approximation theory
- [x] `DirichletCharacter/` - Dirichlet characters and their properties
- [x] `EulerProduct/` - Euler product formulas for L-functions
- [x] `FLT/` - Fermat's Last Theorem related infrastructure
- [x] `Harmonic/` - Harmonic numbers and series
- [x] `Height/` - Height functions in Diophantine geometry
- [x] `JacobiSum/` - Jacobi sums
- [x] `LSeries/` - L-series theory (Dirichlet, Riemann zeta, Hurwitz zeta, analytic continuation)
- [x] `LegendreSymbol/` - Legendre and Jacobi symbols, quadratic reciprocity
- [x] `LocalField/` - Local field theory
- [x] `ModularForms/` - Modular forms and their q-expansions
- [x] `MulChar/` - Multiplicative characters
- [x] `NumberField/` - Algebraic number fields (ideals, class groups, adele rings, infinite places, units)
- [x] `Padics/` - p-adic numbers, valuations, Hensel's lemma, Mahler basis
- [x] `RamificationInertia/` - Ramification and inertia in field extensions
- [x] `Real/` - Real number-theoretic constructions
- [x] `Transcendental/` - Transcendental number theory
- [x] `Zsqrtd/` - Integer rings of quadratic number fields ℤ[√d]

## Search Tags

number-theory primes divisibility factorization arithmetic-functions mobius dirichlet modular-forms L-series riemann-zeta p-adic algebraic-number-theory class-number pell-equation diophantine bertrand lucas-lehmer mersenne-primes quadratic-reciprocity legendre-symbol cyclotomic euler-product continued-fractions perfect-numbers smooth-numbers sieve-methods transcendental adeles ideles valuations ramification
