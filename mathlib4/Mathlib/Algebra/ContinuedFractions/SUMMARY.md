---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/ContinuedFractions
generated: 2025-12-04T13:51:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 1
---

# ContinuedFractions

## Overview

This directory implements comprehensive theory for continued fractions in Lean 4, covering both theoretical foundations and practical computation. The theory encompasses three types: generalized continued fractions (GCF), simple continued fractions (SCF), and regular continued fractions (RCF). The theoretical development provides two equivalent methods for computing convergents (direct evaluation via `convs'` and recurrence relation via `convs`), establishes fundamental properties (recurrence relations for continuants, determinant formula `Aₙ * Bₙ₊₁ - Bₙ * Aₙ₊₁ = (-1)^(n + 1)`), and proves their equivalence following Hardy's proof. The computational side implements the standard algorithm (repeated floor/fractional decomposition) for linear ordered floor fields, proves correctness and convergence with explicit error bounds (`|v - Aₙ/Bₙ| ≤ 1/(Bₙ * Bₙ₊₁)`), establishes the Fibonacci lower bound `Bₙ ≥ Fib(n+1)` for denominators, and characterizes termination: `GenContFract.of v` terminates if and only if `v` is rational. Together, this provides a complete formalization from the mathematical theory through to verified computation.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions for generalized/simple/regular continued fractions, `GenContFract.Pair` structure for partial numerators/denominators, and two methods for computing convergents (`convs` via recurrence, `convs'` via direct evaluation) |
| ContinuantsRecurrence.lean | Proves the recurrence relations for continuants: `Aₙ = bₙ * Aₙ₋₁ + aₙ * Aₙ₋₂` and `Bₙ = bₙ * Bₙ₋₁ + aₙ * Bₙ₋₂` for all n ≥ 1 |
| ConvergentsEquiv.lean | Proves equivalence of the two convergent computation methods (`convs` and `convs'`) via induction and "squashing" technique, following Hardy's proof from *Introduction to the Theory of Numbers* |
| Determinant.lean | Derives the determinant formula for simple continued fractions: `Aₙ * Bₙ₊₁ - Bₙ * Aₙ₊₁ = (-1)^(n + 1)`, with TODO to generalize for GCF |
| TerminatedStable.lean | Theory of terminated continued fractions and stability properties when the sequence terminates |
| Translations.lean | Translation operations and transformations for continued fractions |

## Subdirectories

- [x] `Computation/` - Computable continued fractions for linear ordered floor fields, including the standard algorithm (repeated floor/fractional decomposition), correctness proofs, convergence theory, error bounds (`\|v - Aₙ/Bₙ\| ≤ 1/(Bₙ * Bₙ₊₁)`), and connection to Fibonacci numbers (`Bₙ ≥ Fib(n+1)`)

## Search Tags

continued-fractions generalized-continued-fractions convergents numerics approximation number-theory hardy recurrence-relations determinant-formula fibonacci floor-field rational-approximation
