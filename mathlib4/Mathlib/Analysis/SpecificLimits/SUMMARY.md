---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecificLimits
generated: 2025-12-07T12:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 6
subdirs_count: 0
---

# SpecificLimits

## Overview

This directory contains a collection of specific limit computations and convergence results for various mathematical contexts. The results span basic limits in metric spaces and ordered fields, limits involving normed spaces, arithmetic-geometric sequences, Fibonacci number ratios, and discretized exponentials. By design, `Basic.lean` is independent of `NormedSpace` in the import hierarchy, while `Normed.lean` provides computations that naturally involve normed space theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Fundamental limit computations independent of normed spaces; includes limits like `1/n → 0`, `C/n → 0`, and `1/(n+1) → 0` for various number types (ℕ, ℚ≥0, ℝ, EReal, division semirings with characteristic zero) |
| Normed.lean | Limit computations in (semi-)normed groups/rings/spaces; includes coboundedness of natural/integer casts, asymptotic comparisons of powers (`r₁^n =o[atTop] r₂^n` when `|r₁| < |r₂|`), polynomial growth rates, and convergence of geometric series |
| ArithmeticGeometric.lean | Arithmetic-geometric sequences with recurrence `u(n+1) = a·u(n) + b`; proves closed form `u(n) = a^n·(u₀ - b/(1-a)) + b/(1-a)` for `a ≠ 1`, and convergence results: tends to `+∞` when `1 < a` and `b/(1-a) < u₀`, or to `b/(1-a)` when `0 ≤ a < 1` |
| Fibonacci.lean | Proves that the ratio of consecutive Fibonacci numbers `fib(n+1)/fib(n)` tends to the golden ratio φ as `n → ∞`, and `fib(n)/fib(n+1)` tends to `-ψ` (negative golden ratio conjugate) |
| FloorPow.lean | Results on discretized exponentials of the form `⌊c^n⌋₊`; proves that if monotone sequence `u` satisfies `u(⌊c^n⌋₊)/⌊c^n⌋₊ → l` for all `c > 1`, then `u(n)/n → l`; also provides bounds on sums like `∑_{i≥j} 1/⌊c^i⌋₊²` |
| RCLike.lean | Limit computations for types satisfying `RCLike` (abstraction over ℝ and ℂ); proves coboundedness tendencies for `ofReal` embeddings from ℝ into any `RCLike` type |

## Subdirectories

*(No subdirectories)*

## Search Tags

limits convergence specific-limits asymptotic-analysis fibonacci golden-ratio arithmetic-geometric-sequences discretized-exponentials floor-power p-series geometric-series tendsto normed-spaces metric-spaces ordered-fields division-semirings rclike real-analysis cobounded powers polynomial-growth
