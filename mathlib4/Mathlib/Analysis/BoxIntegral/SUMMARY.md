---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/BoxIntegral
generated: 2025-12-04T17:20:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 2
---

# BoxIntegral

## Overview

The `BoxIntegral/` directory provides a comprehensive formalization of box integral theory, offering a unified framework for multiple integration theories including Riemann, Henstock-Kurzweil, McShane, and GP integrals over rectangular boxes in ℝⁿ. The implementation is built on a foundation of rectangular boxes represented as products of half-open intervals `(l i, u i]` (defined in `Box/`), with rich partition machinery (in `Partition/`) that supports 8 different integration theories through Boolean flags controlling Riemann bounds, Henstock tagging, and distortion constraints. The directory's main files establish integral sums as limits along filters, prove fundamental theorems including the divergence theorem for Henstock-Kurzweil integration and the equivalence between McShane and Bochner integrability, and provide applications to lattice point counting and volume approximation via unit partitions. The architecture separates concerns cleanly: `Box/` handles geometric box operations and induction principles, `Partition/` provides the combinatorial partition framework with box-additive maps, and the top-level files build integration theories on these foundations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Main entry point defining box integrals for Riemann, Henstock-Kurzweil, and McShane theories; defines integral sums, `HasIntegral` predicate, and `integral` function; proves basic properties (linearity, constant functions), Henstock-Sacks inequality, and integrability of continuous functions |
| DivergenceTheorem.lean | Proves the divergence theorem for Henstock-Kurzweil integral: for differentiable `f : ℝⁿ → Eⁿ` on a box, the divergence is integrable and equals the sum of face integrals with appropriate signs; uses a generalized HK integral that restricts box distortion to avoid "long thin" boxes |
| Integrability.lean | Proves equivalence between McShane integrability and Bochner integrability: any Bochner integrable function is McShane (hence Henstock and GP) integrable with the same integral; includes integrability of indicator functions of measurable sets |
| UnitPartition.lean | Defines unit partitions: dividing the unit box into boxes of side length `1/n` translated by integer vectors; proves that sums over lattice points `s ∩ n⁻¹ • (ι → ℤ)` tend to integrals as `n → ∞`, and that lattice point counts approximate volumes |

## Subdirectories

- [x] `Box/` - Rectangular box data structure and operations
- [x] `Partition/` - Partitions and tagged partitions of boxes

## Search Tags

box-integral henstock-kurzweil riemann-integral mcshane-integral integration rectangular-boxes partitions tagged-partitions integral-sum divergence-theorem bochner-integral lattice-points unit-partition volume-approximation real-analysis multivariable-calculus
