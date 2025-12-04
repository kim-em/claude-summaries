---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/ContinuedFractions/Computation
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# Computation

## Overview

This directory implements the standard algorithm for computing continued fractions from values in linear ordered floor fields. It provides the core algorithm (repeated floor/fractional decomposition), correctness proofs showing the computed fraction equals the original value when it terminates, convergence theory with error bounds, and the fundamental theorem that computation terminates if and only if the value is rational. The implementation follows the classical approach: given value `v`, compute `[⌊v⌋; b₀, b₁, ...]` where subsequent terms come from recursively applying the algorithm to `1/(v - ⌊v⌋)`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core computation algorithm: defines `IntFractPair` structure to store integer/fractional parts `⟨⌊v⌋, v - ⌊v⌋⟩`, implements `IntFractPair.stream` to compute the recursive sequence, and produces `GenContFract.of v` as the final continued fraction |
| Translations.lean | Translation lemmas connecting the computation structures (`IntFractPair.stream`, `IntFractPair.seq1`, `GenContFract.of`), recurrence relations for computing stream values, and proofs that termination propagates correctly between structures |
| CorrectnessTerminating.lean | Correctness proof for terminating computations: defines `compExactValue` to compute exact values from convergents and residuals, proves `v = (GenContFract.of v).convs n` when the fraction terminates at position `n` |
| Approximations.lean | Error bounds and approximation theory: proves all partial numerators equal 1, all partial denominators are positive integers, establishes `Bₙ ≥ Fib(n+1)` (denominators grow at least as fast as Fibonacci), and derives the key error bound `\|v - Aₙ/Bₙ\| ≤ 1/(Bₙ * Bₙ₊₁)` |
| ApproximationCorollaries.lean | Convergence corollaries: proves equivalence of the two convergent computation methods (`convs` and `convs'`) for `GenContFract.of`, establishes the recurrence `(of v).convs (n+1) = ⌊v⌋ + 1/(of (fract v)⁻¹).convs n`, and proves `(GenContFract.of v).convs` converges to `v` in the filter topology |
| TerminatesIffRat.lean | Termination characterization: proves the fundamental theorem that `GenContFract.of v` terminates if and only if `v` corresponds to a rational number `q : ℚ`, and establishes `GenContFract.of v = GenContFract.of q` when `↑v = q` |

## Subdirectories

*(None)*

## Search Tags

continued-fractions computation algorithm floor-field rational-approximation convergence error-bounds fibonacci termination correctness numerics number-theory
