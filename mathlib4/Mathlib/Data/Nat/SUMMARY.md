---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat
generated: 2025-12-09T10:35:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: preliminary
files_count: 34
subdirs_count: 10
---

# Nat

## Overview

The `Nat/` directory contains the foundational theory of natural numbers (ℕ) in mathlib4. It provides basic operations, order properties, recursion principles, divisibility theory, primality, number-theoretic functions (GCD, totient, factorization), modular arithmetic, binary representations, logarithms, square roots, and pairing functions. This directory serves as the computational and proof-theoretic foundation for all natural number reasoning in mathlib, building on Lean's core `Nat` type with both home-baked (non-typeclass) development for foundational use and connections to mathlib's algebraic hierarchy.

## Key Files

| File | Purpose |
|------|---------|
| Init.lean | Core initialization file with basic lemmas, extra recursors (`leRecOn`, `decreasing_induction`, `strong_rec'`), and foundational development independent of mathlib's algebraic hierarchy |
| Basic.lean | Builds on `Init.lean` with additional lemmas depending on mathlib definitions; includes `LinearOrder ℕ` instance |
| Notation.lean | Defines the notation `ℕ` for `Nat` |
| BinaryRec.lean | Binary recursion principles for natural numbers |
| Bits.lean | Properties of binary recursion, bit manipulation, `Nat.bits`, and `Nat.size` functions |
| BitIndices.lean | Operations and properties for bit indices in natural numbers |
| Bitwise.lean | Bitwise operations on natural numbers |
| Pairing.lean | Naturals pairing function mapping ℕ² to ℕ; monotone in both directions, maps `[0, n²-1]` to `[0, n-1]²` |
| ModEq.lean | Modular equivalence relation `a ≡ b [MOD n]` (notation for `a % n = b % n`); includes Chinese Remainder Theorem |
| ChineseRemainder.lean | Chinese Remainder Theorem definitions and theorems for Gödel's Beta function |
| Log.lean | Natural logarithm functions: `log b n` (floor log, greatest k where b^k ≤ n) and `clog b n` (ceil log, least k where n ≤ b^k) |
| Sqrt.lean | Properties of natural number square root function |
| PSub.lean | Partial subtraction (predecessor subtraction) on natural numbers |
| Find.lean | Finding the smallest natural number satisfying a predicate |
| Count.lean | Counting natural numbers satisfying properties |
| EvenOddRec.lean | Recursion principles based on even/odd decomposition |
| Lattice.lean | Lattice structure (sup/inf operations) on natural numbers |
| Periodic.lean | Periodicity properties of functions on natural numbers |
| SuccPred.lean | Successor and predecessor operations and properties |
| Upto.lean | Operations on ranges up to a given natural number |
| WithBot.lean | Natural numbers with a bottom element ⊥ |
| Set.lean | Set-theoretic operations on natural numbers |
| Size.lean | Size and bit-length operations on natural numbers |
| Dist.lean | Distance function on natural numbers |
| Nth.lean | Nth element operations and indexing |
| Hyperoperation.lean | Hyperoperations (generalized exponentiation) on natural numbers |
| MaxPowDiv.lean | Maximum power of a divisor |
| Multiplicity.lean | Multiplicity of prime factors in natural numbers |
| Factors.lean | Prime factorization as a list (`primeFactorsList`); includes uniqueness of prime factorization |
| Squarefree.lean | Squarefree natural numbers (not divisible by any non-unit squares); connection to factorization |
| Totient.lean | Euler's totient function φ(n) counting naturals < n coprime to n; divisor sum formula |
| PrimeFin.lean | Prime numbers in finite ranges |
| PowModTotient.lean | Powers modulo totient (import only, delegates to subdirectory) |
| PartENat.lean | Deprecated: natural numbers with infinity using `Part ℕ` (use `ℕ∞` instead); includes order and addition instances |

## Subdirectories

- [ ] `Cast/` - Casting natural numbers to other numeric types
- [ ] `Choose/` - Binomial coefficients (n choose k)
- [ ] `Digits/` - Digit representations in various bases
- [ ] `Factorial/` - Factorial function and properties
- [ ] `Factorization/` - Prime factorization as multisets and related theory
- [ ] `Fib/` - Fibonacci numbers
- [ ] `GCD/` - Greatest common divisor and related functions
- [ ] `NthRoot/` - Nth root functions
- [ ] `Order/` - Order-theoretic properties and lemmas for natural numbers
- [ ] `Prime/` - Prime numbers and primality testing

## Search Tags

natural-numbers arithmetic divisibility primes factorization totient modular-arithmetic binary bits logarithm square-root pairing gcd recursion number-theory
