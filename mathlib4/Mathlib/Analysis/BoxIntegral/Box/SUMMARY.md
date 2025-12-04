---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/BoxIntegral/Box
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Box

## Overview

The `Box/` directory contains the core definition and operations for rectangular boxes in ℝⁿ, represented as products of half-open intervals `(l i, u i]`. The fundamental `BoxIntegral.Box` structure stores lower and upper corners with a proof that each coordinate satisfies `lower i < upper i`. The directory provides partial order and lattice instances, set coercion, operations like faces and distortion, and a powerful induction principle for proving properties on boxes by splitting them through their centers.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `BoxIntegral.Box` structure and operations: defines boxes as pairs of corners with half-open interval interpretation `(lower, upper]`, provides set coercion, partial order where `I ≤ J` means `I ⊆ J`, lattice instances on `WithBot (Box ι)`, face extraction for hyperfaces, distortion (ratio of edge lengths), interior (`Ioo`), closed box (`Icc`), and convergence results for monotone sequences of boxes |
| SubboxInduction.lean | Induction principle for boxes via center-splitting: defines `splitCenterBox` which divides a box into `2^n` subboxes by hyperplanes through its center; proves `subbox_induction_on'` allowing induction on properties that hold locally near each point and propagate through center-splits |

## Subdirectories

(none)

## Search Tags

rectangular-box box-integral half-open-interval box-structure partial-order lattice box-operations face hyperface distortion box-induction center-splitting subbox-induction real-analysis multivariable-integration
