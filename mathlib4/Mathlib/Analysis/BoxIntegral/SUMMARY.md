---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/BoxIntegral
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 4
subdirs_count: 2
---

# BoxIntegral

## Overview

The `BoxIntegral/` directory contains the formalization of box integral theory, providing a unified framework for Riemann, Henstock-Kurzweil, and McShane integration over rectangular boxes in ℝⁿ. The directory defines rectangular boxes as products of half-open intervals `(l i, u i]`, partitions and tagged partitions of boxes, integral sums, and the integral itself as a limit of integral sums along different filters. Key results include the divergence theorem for Henstock-Kurzweil integration, the equivalence between McShane and Bochner integrability, and applications to counting lattice points and computing volumes using unit partitions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Main entry point defining box integrals for Riemann, Henstock-Kurzweil, and McShane theories; defines integral sums, `HasIntegral` predicate, and `integral` function; proves basic properties (linearity, constant functions), Henstock-Sacks inequality, and integrability of continuous functions |
| DivergenceTheorem.lean | Proves the divergence theorem for Henstock-Kurzweil integral: for differentiable `f : ℝⁿ → Eⁿ` on a box, the divergence is integrable and equals the sum of face integrals with appropriate signs; uses a generalized HK integral that restricts box distortion to avoid "long thin" boxes |
| Integrability.lean | Proves equivalence between McShane integrability and Bochner integrability: any Bochner integrable function is McShane (hence Henstock and GP) integrable with the same integral; includes integrability of indicator functions of measurable sets |
| UnitPartition.lean | Defines unit partitions: dividing the unit box into boxes of side length `1/n` translated by integer vectors; proves that sums over lattice points `s ∩ n⁻¹ • (ι → ℤ)` tend to integrals as `n → ∞`, and that lattice point counts approximate volumes |

## Subdirectories

- [x] `Box/` - Rectangular box data structure and operations (complete)
- [ ] `Partition/` - Partitions and tagged partitions of boxes (pending)

## Search Tags

box-integral henstock-kurzweil riemann-integral mcshane-integral integration rectangular-boxes partitions tagged-partitions integral-sum divergence-theorem bochner-integral lattice-points unit-partition volume-approximation real-analysis multivariable-calculus
