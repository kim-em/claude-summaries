---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Meromorphic
generated: 2025-12-05T06:16:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 8
subdirs_count: 0
---

# Meromorphic

## Overview

The `Meromorphic/` directory formalizes meromorphic functions—functions that are holomorphic except at isolated poles where they may tend to infinity. This includes the fundamental definition of `MeromorphicAt`, characterizations of meromorphy in terms of local normal forms `f z = (z - z₀) ^ n • g z`, orders and divisors of meromorphic functions, principles of isolated zeros, identity principles, factorized rational functions, and trailing coefficients. The directory also proves that the Gamma function is meromorphic on the entire complex plane.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `MeromorphicAt f x` (existence of `n : ℕ` such that `(z - x) ^ n • f z` is analytic at `x`); proves meromorphic functions are closed under addition and scalar multiplication; establishes principle of isolated zeros (either `f` vanishes eventually or never in punctured neighborhoods) |
| Complex.lean | Proves that the complex Gamma function is meromorphic on `ℂ` (meromorphic on `univ`) |
| Divisor.lean | Defines the divisor of a meromorphic function mapping each point to its order (as an integer, or zero if order is infinite); proves compatibility with restrictions to subsets and congruence lemmas for functions agreeing on codiscrete sets |
| FactorizedRational.lean | Studies factorized rational functions of the form `∏ᶠ u, (· - u) ^ d u` where `d : 𝕜 → ℤ`; proves these are meromorphic in normal form with divisor equal to `d`; shows meromorphic functions are equivalent (modulo codiscrete equality) to products of factorized rationals and zero-free analytic functions |
| IsolatedZeros.lean | Establishes principles of isolated zeros and identity principles for meromorphic functions; shows if `f` is meromorphic at `x`, then frequent vanishing implies eventual vanishing in punctured neighborhoods; includes results about vanishing along codiscrete subsets |
| NormalForm.lean | Defines `MeromorphicNFAt` (meromorphic in normal form): functions locally expressible as `(z - x) ^ n • g` where `g` is analytic and nonzero at `x`; provides continuous extension API to pick canonical representatives of equivalence classes under `=ᶠ[codiscreteWithin U]`; characterizes normal form functions as those analytic or having poles with value zero at the pole |
| Order.lean | Defines `meromorphicOrderAt f x` as an element of `ℤ ∪ {∞}` (the unique `n` such that `f z = (z - z₀) ^ n • g z` with `g` analytic and nonzero at `z₀`, or `∞` if `f` vanishes identically near `x`); characterizes order being negative (convergence to infinity), zero (nonzero limit), or positive (convergence to zero) |
| TrailingCoefficient.lean | Defines `meromorphicTrailingCoeffAt f x` as the value `g x` from the normal form presentation `f z = (z - x) ^ n • g z` with `g` analytic; expresses the trailing coefficient as a limit and provides characterization lemmas |

## Subdirectories

(None)

## Search Tags

meromorphic holomorphic complex-analysis poles isolated-zeros divisor order normal-form factorized-rational gamma-function trailing-coefficient analytic-functions punctured-neighborhoods codiscrete-sets identity-principle
