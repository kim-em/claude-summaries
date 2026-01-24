---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/Riemannian
generated: 2026-01-24T22:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Riemannian

## Overview

The `Riemannian/` directory formalizes Riemannian manifolds in Mathlib. A Riemannian manifold is a real smooth manifold whose tangent spaces carry smoothly-varying inner products, with an extended metric structure where distance equals the infimum of path lengths. The library provides the `IsRiemannianManifold I M` typeclass, proves that inner product vector spaces are Riemannian manifolds, and shows how to construct the Riemannian distance from a Riemannian metric structure while preserving the original topology. This is foundational infrastructure for differential geometry on manifolds with metric structure.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Module file that imports all Riemannian dependencies; defines `IsRiemannianManifold` typeclass requiring distance equals infimum of path lengths; provides `riemannianMetricVectorSpace` for inner product spaces; constructs `EMetricSpace.ofRiemannianMetric` from Riemannian structure while preserving topology |
| PathELength.lean | Defines `pathELength` (length of a path as integral of derivative norm); proves reparameterization invariance for monotone/antitone maps; defines `riemannianEDist` as infimum of C^1 path lengths; proves triangle inequality and symmetry for `riemannianEDist`; key lemma `exists_lt_locally_constant_of_riemannianEDist_lt` provides paths locally constant near endpoints for gluing |

## Subdirectories

(none)

## Search Tags

riemannian-manifold riemannian-metric path-length riemannian-distance edist inner-product tangent-space isriemannianmanifold pathelength riemannianedist contmdiff smooth-path geodesic metric-space differential-geometry
