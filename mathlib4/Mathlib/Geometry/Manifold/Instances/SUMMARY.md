---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/Instances
generated: 2026-01-24T20:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Instances

## Overview

The `Instances/` directory provides concrete manifold instances for fundamental spaces in differential geometry. It defines the necessary model spaces, charts, and atlases for: the real line and closed intervals `[x,y]` as 1-dimensional manifolds with boundary, unit spheres in inner product spaces as smooth manifolds via stereographic projection, and the unit circle in `ℂ` as a Lie group. Additionally, it establishes that the units of a complete normed algebra (including the general linear group) form a Lie group. These concrete instances make the abstract manifold machinery applicable to important examples.

## Key Files

| File | Purpose |
|------|---------|
| Real.lean | Defines model spaces for real manifolds: `EuclideanHalfSpace n` for manifolds with boundary, `EuclideanQuadrant n` for manifolds with corners; constructs manifold structure on closed intervals `[x,y]` with boundary `{x,y}`; provides notations `𝓡 n` and `𝓡∂ n` |
| Icc.lean | Proves smoothness of inclusion `Icc x y → ℝ` and projection `ℝ → Icc x y` in the manifold sense; defines unit tangent vectors on intervals; relates smoothness on intervals to smoothness of lifted maps |
| Sphere.lean | Defines stereographic projection from unit spheres; constructs analytic manifold structure on spheres in finite-dimensional inner product spaces; proves coercion to ambient space is smooth; establishes `Circle` (unit circle in `ℂ`) as a Lie group with model `𝓡 1` |
| UnitsOfNormedAlgebra.lean | Constructs Lie group structure on units `Rˣ` of complete normed algebras; uses embedding into `R` as manifold chart; applies to general linear group GL(V) as special case |

## Subdirectories

(none)

## Search Tags

manifold-instance sphere stereographic-projection circle lie-group euclidean-half-space euclidean-quadrant icc-interval closed-interval boundary model-with-corners units normed-algebra general-linear-group real-manifold tangent-space smooth-embedding
