---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/SpecialFunctions/Elliptic
generated: 2025-12-05T08:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# Elliptic

## Overview

The `Elliptic/` directory contains theory for elliptic functions, specifically the Weierstrass ℘-function (Weierstrass p-function). This provides the foundational construction of doubly-periodic meromorphic functions on the complex plane associated with a period lattice. The directory defines period pairs (pairs of linearly independent complex periods), the lattice they generate, and the Weierstrass ℘ function as an infinite series over lattice points with specific convergence properties.

## Key Files

| File | Purpose |
|------|---------|
| Weierstrass.lean | Weierstrass ℘-functions and period lattices; defines `PeriodPair` structure for ℝ-linearly independent complex periods, constructs the period lattice, proves the lattice is discrete and proper, defines the Weierstrass ℘ function as a locally uniformly convergent series, establishes differentiability on non-lattice points, and proves evenness (℘(-z) = ℘(z)) |

## Subdirectories

None

## Search Tags

elliptic-functions weierstrass-p-function weierstrass-℘-function period-lattice doubly-periodic complex-analysis meromorphic-functions lattice discrete-topology z-lattice locally-uniform-convergence differentiability complex-periods weierstrass-p weierstrass
