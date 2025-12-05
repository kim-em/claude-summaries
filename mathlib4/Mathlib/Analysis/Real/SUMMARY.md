---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Real
generated: 2025-12-05T08:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 1
---

# Real

## Overview

The `Real/` directory contains fundamental analysis results specific to the real number system. Core topics include set-theoretic properties (cardinality results connecting ℝ to the continuum), extensions beyond the reals (hyperreal construction via ultraproducts), computational representations (positional digit systems), and spectral analysis for real algebras. The Pi subdirectory provides comprehensive treatment of the constant π, including rigorous numerical bounds with proof tactics, multiple irrationality proofs, and classical infinite series formulas (Leibniz, Wallis, Chudnovsky). Together, these files establish both theoretical foundations (cardinality, nonstandard analysis) and computational tools (digit representations, π approximations) for real analysis.

## Key Files

| File | Purpose |
|------|---------|
| Cardinality.lean | Proves that the reals have cardinality continuum (`#ℝ = 𝔠`); shows every real interval with distinct endpoints has cardinality continuum; uses Cantor function mapping `{0,1}^ℕ → ℝ` via `f ↦ Σ n, f n * (1/3)^n` |
| Hyperreal.lean | Constructs hyperreal numbers `ℝ*` as an ultraproduct of real sequences via germs over the hyperfilter extending the cofinite filter on ℕ; provides field and linear order structure |
| OfDigits.lean | Representation of reals in positional systems; defines `Real.ofDigits` (sequence of digits to real `0.d₀d₁d₂...`) and `Real.digits` (real to digit sequence); proves `ofDigits (digits x b) = x` |
| Spectrum.lean | Spectral properties for elements in real algebras; characterizes spectrum restrictions to non-negative reals, with lemmas on ordering elements by spectral bounds |

## Subdirectories

- [x] `Pi/` - Analysis of π: bounds, irrationality proofs (Cartwright's proof), classical formulas (Leibniz series, Wallis product, Chudnovsky algorithm) (complete)

## Search Tags

real-numbers real-analysis cardinality continuum hyperreals nonstandard-analysis ultraproduct positional-system digits spectrum spectral-theory pi irrational
