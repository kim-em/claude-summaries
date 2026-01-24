---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics/BirkhoffSum
generated: 2025-01-24T20:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# BirkhoffSum

## Overview

This folder formalizes Birkhoff sums and averages, fundamental constructs in ergodic theory. Given a self-map `f : α → α` and an observable `g : α → M`, the Birkhoff sum `birkhoffSum f g n x` computes `∑ k ∈ range n, g (f^[k] x)` - the sum of `g` values along the first `n` points of the orbit of `x` under `f`. The Birkhoff average divides this sum by `n`. These time averages appear in ergodic theorems that relate them to space averages. The folder also develops analytic properties in normed spaces (equicontinuity, convergence) and measure-theoretic properties for quasi-measure-preserving maps.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `birkhoffSum f g n x` as the sum along orbits; proves basic identities for zero, one, successor, addition; shows fixed point behavior (`n • g x`); establishes "almost invariance" property relating sums at `f x` vs `x` |
| Average.lean | Defines `birkhoffAverage R f g n x` as the sum divided by `n` (using a division semiring `R`); proves independence from choice of `R`; establishes analogous properties to Basic.lean including almost-invariance and invariant function behavior |
| NormedSpace.lean | Develops Birkhoff averages in normed spaces over `ℝ` or `ℂ`; proves distance estimates between averages, uniform equicontinuity for Lipschitz `f` and uniformly continuous `g`, closedness of convergence sets; motivated by von Neumann Mean Ergodic Theorem |
| QuasiMeasurePreserving.lean | Proves that if `φ =ᵐ[μ] ψ` (almost everywhere equal) under a quasi-measure-preserving map, then `birkhoffSum f φ n =ᵐ[μ] birkhoffSum f ψ n` and similarly for averages |

## Subdirectories

(none)

## Search Tags

birkhoff-sum birkhoff-average ergodic-theory time-average orbit-sum dynamical-systems measure-preserving quasi-measure-preserving normed-space equicontinuity lipschitz uniform-continuity von-neumann-ergodic-theorem convergence fixed-point iteration
