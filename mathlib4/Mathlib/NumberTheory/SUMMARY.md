---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory
generated: 2026-01-25T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 47
subdirs_count: 21
---

# NumberTheory

## Overview

The `NumberTheory/` directory contains comprehensive formalizations of classical and modern number theory, spanning elementary topics (primality, divisibility, factorization) through advanced theories (L-series, p-adic analysis, algebraic number theory, modular forms). The directory includes major results like Bertrand's postulate, the Lucas-Lehmer primality test for Mersenne primes, Pell's equation solutions, Diophantine equations (including Matiyasevic's theorem), and arithmetic function theory. It provides both computational tools (primality tests, factorization algorithms) and deep theoretical frameworks (class numbers, adele rings, L-functions, p-adic valuations).

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
- [ ] `JacobiSum/` - Jacobi sums
- [ ] `LSeries/` - L-series theory (Dirichlet, Riemann zeta, Hurwitz zeta, analytic continuation)
- [ ] `LegendreSymbol/` - Legendre and Jacobi symbols, quadratic reciprocity
- [ ] `LocalField/` - Local field theory
- [ ] `ModularForms/` - Modular forms and their q-expansions
- [ ] `MulChar/` - Multiplicative characters
- [ ] `NumberField/` - Algebraic number fields (ideals, class groups, adele rings, infinite places, units)
- [ ] `Padics/` - p-adic numbers, valuations, Hensel's lemma, Mahler basis
- [ ] `RamificationInertia/` - Ramification and inertia in field extensions
- [ ] `Real/` - Real number-theoretic constructions
- [ ] `Transcendental/` - Transcendental number theory
- [ ] `Zsqrtd/` - Integer rings of quadratic number fields ℤ[√d]

## Search Tags

number-theory primes divisibility factorization arithmetic-functions mobius dirichlet modular-forms L-series riemann-zeta p-adic algebraic-number-theory class-number pell-equation diophantine bertrand lucas-lehmer mersenne-primes quadratic-reciprocity legendre-symbol cyclotomic euler-product continued-fractions perfect-numbers smooth-numbers sieve-methods transcendental adeles ideles valuations ramification
