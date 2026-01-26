---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Kernel/IonescuTulcea
generated: 2026-01-26T23:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 3
subdirs_count: 0
---

# IonescuTulcea

## Overview

The IonescuTulcea directory contains the formalization of the Ionescu-Tulcea theorem, which constructs measures on infinite product spaces by composing an infinite sequence of kernels. Given a family of kernels κ(n) from trajectories up to time n to distributions at time n+1, the theorem produces a kernel on infinite trajectories. This provides a rigorous foundation for defining Markov processes and stochastic processes with history-dependent transitions.

## Key Files

| File | Purpose |
|------|---------|
| Maps.lean | Auxiliary measurable maps for gluing trajectory intervals: `IocProdIoc` glues half-open intervals, `IicProdIoc` glues closed prefix intervals with half-open extensions, includes measurable equivalences for dependent function types indexed by intervals |
| PartialTraj.lean | Defines `partialTraj κ a b` kernel giving distribution of trajectory up to time b given trajectory up to time a, includes composition properties `partialTraj κ b c ∘ₖ partialTraj κ a b = partialTraj κ a c`, provides `lmarginalPartialTraj` for computing integrals against partial trajectories |
| Traj.lean | Main Ionescu-Tulcea theorem: constructs `traj κ a` kernel from finite trajectories to infinite trajectories using Carathéodory extension, proves uniqueness and integration formulas, includes `trajMeasure` for starting distributions, establishes conditional distribution properties connecting `traj` to the original kernels |

## Subdirectories

## Search Tags

ionescu-tulcea-theorem markov-processes stochastic-processes infinite-products projective-limit caratheodory-extension trajectory-composition kernel-composition probability-kernels measure-theory dependent-kernels conditional-distributions projective-families
