---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/Choose
generated: 2025-12-09T11:30:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 11
subdirs_count: 0
---

# Choose

## Overview

The `Choose/` directory contains the comprehensive theory of binomial coefficients (n choose k) and related combinatorial functions in mathlib4. It provides the core definition via Pascal's triangle recursion, proves the factorial formula, establishes fundamental identities (symmetry, Vandermonde), proves inequalities and bounds (exponential bounds, maximum at middle), relates binomial coefficients to factorizations and primality (Lucas's theorem, Legendre's formula), and extends to generalizations including multichoose (multicombinations/stars-and-bars) and multinomial coefficients. This is the foundational combinatorics for counting k-element subsets, with applications throughout discrete mathematics and number theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and basic properties: `choose n k` via Pascal's triangle, factorial formula `n! / (k! * (n-k)!)`, symmetry `choose n k = choose n (n-k)`, recursion lemmas, relationship to ascending/descending factorials, `multichoose` (multicombinations/stars-and-bars), basic inequalities (middle value maximality) |
| Factorization.lean | Prime factorization properties of binomial coefficients: Legendre's theorem (multiplicity of prime p in n! as sum of n/p^i), logarithmic upper bounds on prime multiplicities, bounds on when primes appear (primes > sqrt(n) appear at most once, primes in (2n/3, n) don't appear in central binomial coefficients) - used in Erdős's proof of Bertrand's postulate |
| Multinomial.lean | Multinomial coefficients counting strings with specified symbol multiplicities: definition as `(∑ f i)! / ∏ (f i)!`, positivity, specification lemma, expansion of `(s.sum x)^n` using multinomial coefficients |
| Sum.lean | Sums of binomial coefficients: binomial theorem for commuting elements `(x+y)^n = ∑ x^m * y^(n-m) * choose n m`, various summation identities and applications |
| Lucas.lean | Lucas's theorem: for prime p, `n choose k ≡ ∏(n_i choose k_i) (mod p)` where n_i, k_i are base-p digits of n, k respectively; proof via polynomial methods |
| Central.lean | Central binomial coefficients `(2n) choose n`: inductive relationship between successive values, exponential lower bound `4^n < (2n choose n) * (n+1)`, divisibility `(n+1) | (2n choose n)` (ensures Catalan numbers are integers) |
| Vandermonde.lean | Vandermonde's identity: `(m+n) choose k = ∑_{i+j=k} (m choose i) * (n choose j)` via algebraic proof using polynomials |
| Bounds.lean | Exponential inequalities: upper bound `choose n r ≤ n^r / r!`, lower bound `(n+1-r)^r / r! ≤ choose n r`, bounds via descending factorial, power-of-two bounds `choose n k < 2^n` |
| Cast.lean | Casting binomial coefficients to division rings of characteristic 0: formula `(choose b a : K) = b! / (a! * (b-a)!)`, specialized formula for `choose a 2` |
| Dvd.lean | Divisibility by primes: conditions for prime p to divide `choose (a+b) a`, `choose p k` for k < p, coprimality results for choose with primes less than denominator |
| Mul.lean | Multiplication lemmas requiring ring tactics: `choose (m*n+n) n = (m+1) * choose (m*n+n-1) (n-1)`, `choose (m*n) n = m * choose (m*n-1) (n-1)` |

## Subdirectories

None.

## Search Tags

binomial-coefficients choose combinations multichoose multinomial pascals-triangle factorial vandermonde lucas-theorem central-binomial catalan-number legendre-formula stars-and-bars counting combinatorics
