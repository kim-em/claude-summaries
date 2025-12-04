---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/AddTorsor
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# AddTorsor

## Overview

The `AddTorsor/` directory contains results about smoothness of functions on affine spaces and torsors (affine spaces without a distinguished origin). It proves that continuous affine maps are smooth (C^∞) and that barycentric coordinates are smooth. This extends the calculus framework to affine geometry, which is essential for working with spaces that lack a canonical zero point.

## Key Files

| File | Purpose |
|------|---------|
| AffineMap.lean | Proves continuous affine maps are smooth: establishes that `ContinuousAffineMap.contDiff` shows affine maps are C^n for all n, and derives differentiability properties with explicit Fréchet derivative formula |
| Coord.lean | Proves barycentric coordinates are smooth: shows `smooth_barycentric_coord` establishes that coordinate functions of an affine basis are C^∞ in finite-dimensional normed spaces |

## Subdirectories

None.

## Search Tags

affine-map affine-space torsor barycentric-coordinates smooth continuously-differentiable contdiff continuous-affine-map fréchet-derivative normed-addtorsor affine-basis
