---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Real
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 4
subdirs_count: 1
---

# Real

## Overview

The `Real/` directory contains analysis specific to the real numbers. This includes fundamental results about cardinality of the reals, hyperreal numbers (ultraproduct construction), positional digit representations, and spectral theory for real algebras. The directory also includes a subdirectory dedicated to π (pi), covering bounds, irrationality proofs, and classical formulas.

## Key Files

| File | Purpose |
|------|---------|
| Cardinality.lean | Proves that the reals have cardinality continuum (`#ℝ = 𝔠`); shows every real interval with distinct endpoints has cardinality continuum; uses Cantor function mapping `{0,1}^ℕ → ℝ` via `f ↦ Σ n, f n * (1/3)^n` |
| Hyperreal.lean | Constructs hyperreal numbers `ℝ*` as an ultraproduct of real sequences via germs over the hyperfilter extending the cofinite filter on ℕ; provides field and linear order structure |
| OfDigits.lean | Representation of reals in positional systems; defines `Real.ofDigits` (sequence of digits to real `0.d₀d₁d₂...`) and `Real.digits` (real to digit sequence); proves `ofDigits (digits x b) = x` |
| Spectrum.lean | Spectral properties for elements in real algebras; characterizes spectrum restrictions to non-negative reals, with lemmas on ordering elements by spectral bounds |

## Subdirectories

- [ ] `Pi/` - Analysis of π: bounds, irrationality proofs (Cartwright's proof), classical formulas (Leibniz series, Wallis product, Chudnovsky algorithm) (pending)

## Search Tags

real-numbers real-analysis cardinality continuum hyperreals nonstandard-analysis ultraproduct positional-system digits spectrum spectral-theory pi irrational
