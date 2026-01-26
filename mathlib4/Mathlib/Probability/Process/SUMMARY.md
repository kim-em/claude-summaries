---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Process
generated: 2026-01-26T20:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 8
subdirs_count: 0
---

# Process

## Overview

The `Process/` directory provides formalization of stochastic processes and their core properties. It defines fundamental concepts including filtrations (sequences of σ-algebras), adapted and progressively measurable processes, stopping times, hitting times, and predictable processes. The directory includes the machinery for working with discrete-time and continuous-time stochastic processes, with support for the Kolmogorov-Chentsov theorem conditions and finite-dimensional distributions. This provides the foundation for probability theory and martingale theory in Mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Filtration.lean | Defines filtrations (monotone sequences of sub-σ-algebras), σ-finite filtrations, natural filtrations from processes, right-continuous filtrations, limit processes, and the canonical product filtration on `Π i, X i` |
| Adapted.lean | Defines adapted, strongly adapted, and progressively measurable processes with respect to filtrations; proves continuous strongly adapted processes are progressively measurable |
| Stopping.lean | Defines stopping times as functions `Ω → WithTop ι` satisfying the stopping time property, the σ-algebra associated with a stopping time, stopped processes, and proves stopped processes of progressively measurable processes are progressively measurable |
| HittingTime.lean | Defines hitting times `hittingBtwn` (first time process enters a set in an interval) and `hittingAfter` (first time process enters a set after some time), proves hitting times are stopping times for discrete strongly adapted processes |
| Predictable.lean | Defines the predictable σ-algebra for filtrations and predictable processes (measurable with respect to predictable σ-algebra), proves predictable processes are progressively measurable and adapted |
| FiniteDimensionalLaws.lean | Defines finite-dimensional distributions of stochastic processes via `P.map (fun ω ↦ I.restrict (X · ω))`, proves processes have the same law iff they have the same finite-dimensional distributions (via projective limit theory) |
| Kolmogorov.lean | Defines `IsKolmogorovProcess` (processes satisfying the Kolmogorov condition `∫⁻ ω, edist (X s ω) (X t ω) ^ p ∂P ≤ M * edist s t ^ q`), used for the Kolmogorov-Chentsov theorem on continuous modifications |
| PartitionFiltration.lean | Defines filtrations built from finite partitions (`partitionFiltration` from arbitrary partitions, `countableFiltration` from countable partitions in countably generated spaces), used for constructing measurable functions via martingale convergence |

## Subdirectories

(none)

## Search Tags

stochastic-process filtration adapted progressively-measurable stopping-time hitting-time predictable kolmogorov finite-dimensional-laws projective-limit measure-theory sigma-algebra measurable-space
