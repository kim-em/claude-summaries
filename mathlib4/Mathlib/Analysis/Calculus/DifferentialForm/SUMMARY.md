---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/DifferentialForm
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# DifferentialForm

## Overview

The `DifferentialForm/` directory contains the formalization of differential forms on normed spaces and their exterior derivatives. It defines the exterior derivative operator `dω`, proves fundamental properties (linearity, d²=0), and establishes the relationship between exterior derivatives and pullbacks under smooth maps. Differential `n`-forms are represented as `E → E [⋀^Fin n]→L[𝕜] F` (functions from points to alternating continuous multilinear maps).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines exterior derivative (extDeriv) and exterior derivative within a set (extDerivWithin); proves linearity, that the second exterior derivative is zero (d²=0), formula for applying exterior derivatives to vectors, congruence lemmas for eventually equal forms, special cases for 0-forms and 1-forms, and pullback compatibility under smooth maps |

## Subdirectories

*(none)*

## Search Tags

differential-forms exterior-derivative exterior-calculus de-rham-complex alternating-forms normed-spaces fréchet-derivative pullback differential-geometry cartan-formula smoothness continuously-differentiable uniquediffwithinat
