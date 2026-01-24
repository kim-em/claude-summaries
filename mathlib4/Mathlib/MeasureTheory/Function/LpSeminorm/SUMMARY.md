---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function/LpSeminorm
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# LpSeminorm

## Overview

The `LpSeminorm/` directory contains the foundational theory of Lp seminorms in measure theory. It defines the eLpNorm function `‖f‖_p = (∫ ‖f‖^p dμ)^(1/p)` for 0 < p < ∞ and `‖f‖_∞ = essSup ‖f‖` for p = ∞, establishes the triangle inequality and other seminorm properties, provides comparison inequalities between different exponents, proves the Chebyshev-Markov inequality in the Lp context, and studies how Lp seminorms behave under measure restriction, product measures, and trimming to sub-σ-algebras. This forms the analytical foundation for the Lp space constructions in the parent `LpSpace/` directory.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: eLpNorm', eLpNormEssSup, eLpNorm (the Lp seminorm), and MemLp predicate (almost everywhere strongly measurable with finite p-seminorm) |
| Basic.lean | Fundamental properties of Lp seminorms: behavior at zero, positivity, homogeneity, monotonicity, relations between eLpNorm variants, and basic finiteness criteria |
| TriangleInequality.lean | Triangle inequality for Lp seminorms: ‖f + g‖_p ≤ C(‖f‖_p + ‖g‖_p) where C = 1 for p ≥ 1 and C = 2^(1/p-1) for 0 < p < 1, with corollaries for sums |
| CompareExp.lean | Comparison inequalities between Lp norms with different exponents: ‖f‖_p ≤ ‖f‖_q · μ(univ)^(1/p - 1/q) for p ≤ q, with specialized versions for probability measures |
| ChebyshevMarkov.lean | Chebyshev-Markov inequality in Lp form: bounds on μ{x : ε ≤ ‖f(x)‖} in terms of ‖f‖_p, useful for tail probability estimates |
| Prod.lean | Behavior of Lp seminorms under product measures: if f ∈ Lp(μ), then f ∘ fst ∈ Lp(μ × ν) when ν is finite |
| Trim.lean | Lp seminorms with respect to restricted measures: ‖f‖_{Lp(μ.trim)} = ‖f‖_{Lp(μ)} when f is measurable with respect to the smaller σ-algebra |

## Subdirectories

None

## Search Tags

lp-seminorm elpnorm memlp triangle-inequality chebyshev-markov-inequality holder-exponent seminorm-comparison measure-trim product-measure essential-supremum finite-seminorm ae-strongly-measurable lp-space-theory
