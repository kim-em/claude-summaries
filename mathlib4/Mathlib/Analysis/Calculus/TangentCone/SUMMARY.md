---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/TangentCone
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# TangentCone

## Overview

The `TangentCone/` subdirectory contains the formalization of tangent cones and the unique differentiability property for sets in normed spaces. The tangent cone `tangentConeAt 𝕜 s x` is the set of all tangent directions to set `s` at point `x`, defined via sequences of rescaled points converging to the point. The main application is ensuring uniqueness of derivatives: when the span of the tangent cone is dense, any two derivatives at that point must coincide. This directory proves basic properties of tangent cones (monotonicity, behavior under closures and products), characterizes unique differentiability in special settings (dimension one, products, pi types, convex sets, real intervals), and establishes nontriviality of tangent cones in proper spaces.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `tangentConeAt 𝕜 s x` (set of tangent directions as limits of rescaled sequences), `UniqueDiffWithinAt` (predicate ensuring derivative uniqueness via dense span of tangent cone), and `UniqueDiffOn` (unique differentiability at all points of a set) |
| Basic.lean | Proves basic properties of tangent cones: monotonicity under set inclusion and field extension, behavior under closures and neighborhoods, contains zero at accumulation points, product subsets zero at non-accumulation points; proves basic properties of UniqueDiffWithinAt (monotonicity, behavior under intersections and closures, open sets have unique diff) |
| DimOne.lean | Characterizes unique differentiability in dimension one: proves tangent cone at accumulation point equals entire space, establishes `uniqueDiffWithinAt_iff_accPt` (unique differentiability iff accumulation point) |
| Pi.lean | Proves that finite indexed products of sets with unique differentiability property inherit the property; shows tangent cone of product contains images of factor tangent cones via coordinate injections |
| Prod.lean | Proves that binary products of sets with unique differentiability property have the property; establishes tangent cone of product contains left and right factor tangent cones via linear injections |
| ProperSpace.lean | Proves tangent cone at accumulation point in proper normed space is nontrivial (contains nonzero elements); uses compactness to extract convergent subsequence from rescaled sequences |
| Real.lean | Proves unique differentiability for convex sets with nonempty interior in real normed spaces (via open segments in tangent cone); establishes unique differentiability for all real intervals (Ici, Iic, Ioi, Iio, Icc, Ico, Ioc, Ioo) using convexity |

## Subdirectories

(No subdirectories)

## Search Tags

tangent-cone unique-differentiability derivatives derivative-uniqueness normed-spaces accumulation-points convex-sets real-intervals products pi-types proper-spaces dense-span closure monotonicity open-segments calculus
