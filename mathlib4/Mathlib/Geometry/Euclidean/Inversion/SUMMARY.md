---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Euclidean/Inversion
generated: 2026-01-24T07:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Inversion

## Overview

This directory formalizes geometric inversion (circle inversion) in Euclidean affine spaces. Inversion in a sphere sends each point `x` to a point `y` such that `y - c = (R / dist x c)^2 * (x - c)`, where `c` is the center and `R` is the radius. The library establishes that inversion is an involution (applying it twice returns the original point), proves formulas for distances under inversion, derives Ptolemy's inequality using inversion, provides calculus results (derivatives, smoothness), and shows how inversion transforms spheres passing through the center into hyperplanes.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `inversion c R x` and fundamental properties: involutivity, bijectivity, distance formulas, triangle similarity under inversion, and proof of Ptolemy's inequality |
| Calculus.lean | Differentiability and smoothness (`ContDiff`) of inversion; explicit formula for the Frechet derivative involving reflection across the orthogonal complement |
| ImageHyperplane.lean | Image of spheres and hyperplanes under inversion: spheres through the center map to hyperplanes (perpendicular bisectors), and affine subspaces through the center are preserved |

## Subdirectories

(none)

## Search Tags

inversion circle-inversion sphere-inversion involutive ptolemy-inequality ptolemy distance-formula affine-space inner-product-space derivative frechet-derivative contdiff differentiable hyperplane perpendicular-bisector reflection similarity
