---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/Fib
generated: 2025-12-11T00:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 2
subdirs_count: 0
---

# Fib

## Overview

The `Fib/` directory provides the theory of Fibonacci numbers in mathlib4. It defines the Fibonacci sequence `F₀ = 0, F₁ = 1, Fₙ₊₂ = Fₙ + Fₙ₊₁` and proves fundamental properties including the recurrence relation, monotonicity, coprimality of consecutive terms, the strong divisibility property (`gcd(Fₘ, Fₙ) = F_gcd(m,n)`), and the connection to binomial coefficients via antidiagonals. It also includes an efficient O(log n) algorithm for computing Fibonacci numbers using binary representation, and proves Zeckendorf's theorem: every natural number has a unique representation as a sum of non-consecutive Fibonacci numbers.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core Fibonacci sequence definition via stream iteration; proves recurrence, monotonicity, coprimality of consecutive terms, strong divisibility (`fib_gcd`), sum formulas, binomial coefficient connection (`fib_succ_eq_sum_choose`), and fast O(log n) computation via binary representation (`fastFib`) |
| Zeckendorf.lean | Zeckendorf's theorem: every natural has a unique representation as sum of non-consecutive Fibonacci numbers; defines `IsZeckendorfRep` predicate, `greatestFib` function, `zeckendorf` representation algorithm, and `zeckendorfEquiv` equivalence |

## Subdirectories

(none)

## Search Tags

fibonacci fibonacci-sequence zeckendorf representation fast-doubling gcd coprime divisibility monotone binomial-coefficients number-theory
