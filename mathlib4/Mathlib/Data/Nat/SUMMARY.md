---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat
generated: 2025-12-11T23:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 34
subdirs_count: 10
---

# Nat

## Overview

The `Nat/` directory contains the comprehensive theory of natural numbers (ℕ) in mathlib4, serving as the foundational number-theoretic infrastructure upon which most of mathlib is built. The development spans from basic arithmetic and recursion principles to advanced number theory including primality, factorization, and modular arithmetic.

**Core foundations**: The `Init.lean` and `Basic.lean` files establish fundamental lemmas, extra recursors (`leRecOn`, `decreasing_induction`, `strong_rec'`), and the `LinearOrder ℕ` instance. This "home-baked" development avoids typeclass dependencies for foundational use while connecting to mathlib's algebraic hierarchy.

**Binary and bit operations**: The `BinaryRec.lean`, `Bits.lean`, `BitIndices.lean`, and `Bitwise.lean` files provide binary recursion principles, bit manipulation, and bitwise operations on natural numbers.

**Arithmetic functions**: Core number-theoretic functions include logarithms (`Log.lean`: floor and ceiling log), square roots (`Sqrt.lean`), distance (`Dist.lean`), and hyperoperations (`Hyperoperation.lean`). The `Pairing.lean` file implements Cantor's pairing function ℕ² → ℕ.

**Divisibility and primality**: The `Prime/` subdirectory defines `Nat.Prime` as `Irreducible`, provides `minFac` for computing smallest prime factors, proves Euclid's infinitude theorem, and connects to factorial divisibility. The `Factorization/` subdirectory represents prime factorizations as `ℕ →₀ ℕ` (primes to multiplicities), enabling algebraic manipulation and induction principles. Related files include `Factors.lean` (factorization as lists), `Squarefree.lean`, `Multiplicity.lean`, and `MaxPowDiv.lean`.

**Modular arithmetic**: The `ModEq.lean` and `ChineseRemainder.lean` files develop modular equivalence and the Chinese Remainder Theorem (including Gödel's Beta function). Euler's totient function appears in `Totient.lean`.

**Combinatorics**: The `Choose/` subdirectory provides binomial coefficients via Pascal's triangle, the factorial formula, Lucas's theorem, Vandermonde's identity, and multinomial coefficients. The `Factorial/` subdirectory defines factorial variants (ascending, descending, double, superfactorial) with efficient binary-splitting implementations.

**Sequences and special numbers**: The `Fib/` subdirectory covers Fibonacci numbers with fast O(log n) computation and Zeckendorf's theorem. The `Digits/` subdirectory provides base-b digit extraction and classical divisibility tests.

**Casting and coercion**: The `Cast/` subdirectory implements the canonical homomorphism from ℕ to algebraic structures, enabling numeric literals like `37 : R` in any ring.

**Order and lattice**: The `GCD/` subdirectory develops gcd/lcm theory and coprimality, while `Order/` provides order-theoretic lemmas and lattice instances for subtypes of naturals.

## Key Files

| File | Purpose |
|------|---------|
| Init.lean | Core initialization: basic lemmas, extra recursors (`leRecOn`, `decreasing_induction`, `strong_rec'`), foundational development independent of algebraic hierarchy |
| Basic.lean | Additional lemmas depending on mathlib definitions; `LinearOrder ℕ` instance |
| Notation.lean | Defines the notation `ℕ` for `Nat` |
| BinaryRec.lean | Binary recursion principles for natural numbers |
| Bits.lean | Binary recursion properties, bit manipulation, `Nat.bits`, `Nat.size` |
| BitIndices.lean | Operations and properties for bit indices |
| Bitwise.lean | Bitwise operations (and, or, xor, etc.) |
| Pairing.lean | Cantor pairing function ℕ² → ℕ; monotone, bijective |
| ModEq.lean | Modular equivalence `a ≡ b [MOD n]`; Chinese Remainder Theorem |
| ChineseRemainder.lean | CRT definitions for Gödel's Beta function |
| Log.lean | Floor log `log b n` and ceiling log `clog b n` |
| Sqrt.lean | Natural number square root properties |
| PSub.lean | Partial/predecessor subtraction |
| Find.lean | Finding smallest natural satisfying a predicate |
| Count.lean | Counting naturals satisfying properties |
| EvenOddRec.lean | Recursion via even/odd decomposition |
| Lattice.lean | Lattice structure (sup/inf) on naturals |
| Periodic.lean | Periodicity of functions on naturals |
| SuccPred.lean | Successor and predecessor operations |
| Upto.lean | Operations on ranges up to n |
| WithBot.lean | Natural numbers with bottom element ⊥ |
| Set.lean | Set-theoretic operations on naturals |
| Size.lean | Size and bit-length operations |
| Dist.lean | Distance function |
| Nth.lean | Nth element operations and indexing |
| Hyperoperation.lean | Generalized exponentiation (hyperoperations) |
| MaxPowDiv.lean | Maximum power of a divisor |
| Multiplicity.lean | Prime multiplicity in natural numbers |
| Factors.lean | Prime factorization as list (`primeFactorsList`); uniqueness |
| Squarefree.lean | Squarefree naturals; factorization connection |
| Totient.lean | Euler's totient φ(n); divisor sum formula |
| PrimeFin.lean | Primes in finite ranges |
| PowModTotient.lean | Powers modulo totient (import delegation) |
| PartENat.lean | Deprecated: naturals with infinity via `Part ℕ` (use `ℕ∞`) |

## Subdirectories

- [x] `Cast/` - Canonical homomorphism from ℕ to algebraic structures; `NatCast`, `AddMonoidWithOne` typeclasses; field casting; order properties
- [x] `Choose/` - Binomial coefficients via Pascal's triangle; factorial formula; Lucas's theorem; Vandermonde's identity; multinomial coefficients; central binomial coefficients
- [x] `Digits/` - Base-b digit extraction (`digits`, `ofDigits`); divisibility tests for 3, 9, 11; modular arithmetic properties
- [x] `Factorial/` - Factorial `n!`, ascending/descending factorials, double factorial `n!!`, superfactorial; binary-splitting computation; casting lemmas
- [x] `Factorization/` - Prime factorization as `ℕ →₀ ℕ`; `ordProj`/`ordCompl`; floor/ceiling roots; induction principles; prime power characterization
- [x] `Fib/` - Fibonacci numbers; strong divisibility `gcd(Fₘ, Fₙ) = F_{gcd(m,n)}`; fast O(log n) computation; Zeckendorf's theorem
- [x] `GCD/` - Greatest common divisor and least common multiple; coprimality lemmas; prime interactions; big operator products
- [x] `NthRoot/` - Floor of nth root via Newton's method
- [x] `Order/` - Order-theoretic lemmas; `OrderBot`/`SemilatticeSup` for subtypes; set characterization
- [x] `Prime/` - `Nat.Prime` definition; `minFac`; Euclid's infinitude theorem; factorial interactions; integer connection

## Search Tags

natural-numbers arithmetic divisibility primes prime-factorization factorization totient euler-phi modular-arithmetic chinese-remainder binary bits bitwise logarithm square-root pairing gcd lcm coprime recursion induction fibonacci zeckendorf binomial-coefficients choose factorial multinomial digits base-representation casting coercion number-theory
