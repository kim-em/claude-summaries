---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/Conformal
generated: 2025-12-04T21:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Conformal

## Overview

The `Conformal/` directory formalizes conformal maps—differentiable maps whose derivatives preserve angles (or equivalently, scale distances uniformly in all directions). It provides the main definitions of `ConformalAt` (conformality at a point) and `Conformal` (globally conformal), characterizations in terms of inner products for inner product spaces, and the conformal factor. Note that the definition does NOT require orientation preservation; complex conjugation is considered conformal.

## Key Files

| File | Purpose |
|------|---------|
| NormedSpace.lean | Main definitions of conformal maps on normed spaces; `ConformalAt f x` means f has a conformal differential at x; proves conformality of identity, scalar multiplication, and compositions; characterizes conformality via `IsConformalMap` of the Fréchet derivative |
| InnerProduct.lean | Characterization of conformality in inner product spaces; proves `conformalAt_iff'`: f is conformal at x iff its differential scales all inner products by a positive constant; defines `conformalFactorAt` (the scaling constant) |

## Subdirectories

None.

## Search Tags

conformal-maps angle-preserving differentiable-maps conformal-factor inner-product-spaces fréchet-derivative isometric-scaling local-conformality global-conformality
