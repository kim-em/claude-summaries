---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/Factorial
generated: 2025-12-11T10:45:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 6
subdirs_count: 0
---

# Factorial

## Overview

The `Factorial/` directory defines the factorial function and its variants for natural numbers in mathlib4. It includes the standard factorial `n!`, ascending factorial `n.ascFactorial k` (product from n to n+k-1), descending factorial `n.descFactorial k` (product from n-k+1 to n), double factorial `n!!` (product of every other number), and superfactorial `sf n` (product of all factorials up to n!). The directory also provides efficient binary-splitting implementations for computation, casting lemmas for evaluating factorials in semirings, and conditions for when factorial casts are units.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and properties: `Nat.factorial`, `Nat.ascFactorial`, `Nat.descFactorial`; notation `n!`; divisibility, monotonicity, injectivity lemmas; bounds relating factorials to powers; binary-splitting implementations (`factorialBinarySplitting`, `ascFactorialBinary`, `descFactorialBinary`) marked with `@[csimp]` for efficient computation |
| BigOperators.lean | Lemmas connecting factorials to `Finset.prod`: `factorial_eq_prod_range_add_one`, `ascFactorial_eq_prod_range`, `descFactorial_eq_prod_range`; `factorial_coe_dvd_prod` showing k! divides product of k consecutive integers |
| Cast.lean | Casting descending factorial to rings: `cast_descFactorial_two` expressing `(a.descFactorial 2 : S) = a * (a - 1)` using true subtraction rather than truncated natural subtraction |
| DoubleFactorial.lean | Double factorial `n!! = n * (n-2) * (n-4) * ...`; notation `n!!`; relationship to factorial via `factorial_eq_mul_doubleFactorial`; product formulas for even and odd cases; positivity extension for the `positivity` tactic |
| NatCast.lean | Conditions for `(n! : A)` to be a unit: `IsUnit.natCast_factorial_of_algebra` for char-zero algebras, `IsUnit.natCast_factorial_iff_of_charP` for characteristic p (unit iff n < p), `IsUnit.natCast_factorial_of_isNilpotent` when p is nilpotent; `Nat.castChoose_eq` for computing binomial coefficients via inverses |
| SuperFactorial.lean | Superfactorial `sf n = 1! * 2! * ... * n!`; product formulas `prod_Icc_factorial`, `prod_range_factorial_succ`; identities for `superFactorial_two_mul` and `superFactorial_four_mul` |

## Subdirectories

*(none)*

## Search Tags

factorial ascending-factorial descending-factorial double-factorial superfactorial combinatorics natural-numbers binomial-coefficients pochhammer binary-splitting computation cast unit invertible
