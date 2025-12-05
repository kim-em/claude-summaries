---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Complex/Harmonic
generated: 2025-12-05T01:28:36Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Harmonic

## Overview

The `Harmonic/` directory contains the theory of harmonic functions on the complex plane—functions satisfying Laplace's equation. It establishes the fundamental connection between harmonicity and complex analyticity, proving that harmonic functions are real parts of holomorphic functions and are therefore real-analytic. The main results include the analyticity of the complex partial derivative operator and the mean value property for harmonic functions.

## Key Files

| File | Purpose |
|------|---------|
| Analytic.lean | Proves harmonic functions are real-analytic by showing they are real parts of holomorphic functions; establishes analyticity of ∂f/∂1 - I • ∂f/∂I for harmonic f |
| MeanValue.lean | The mean value property: for harmonic f on a closed disc, the circle average equals the center value f(c) |

## Subdirectories

None.

## Search Tags

harmonic-functions laplace-equation real-analytic holomorphic-functions mean-value-property circle-average complex-partial-derivative cauchy-riemann harmonic-conjugate analyticity inner-product-space
