---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/SimplexCategory/Augmented
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Augmented

## Overview

The `Augmented/` directory defines the augmented simplex category, which extends the standard simplex category by adjoining an initial object. This construction is fundamental in simplicial homotopy theory. The directory establishes equivalences between functors out of the augmented simplex category and augmented (co)simplicial objects, and equips the augmented simplex category with a monoidal structure where the initial object serves as the unit and tensor products correspond to ordinal sums.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `AugmentedSimplexCategory` as `WithInitial SimplexCategory`, provides the canonical inclusion functor, proves equivalences between functors from augmented simplex category and augmented (co)simplicial objects, and establishes relationships between drop/point/toArrow operations |
| Monoidal.lean | Defines monoidal structure on `AugmentedSimplexCategory` where the initial object is the unit, tensor products satisfy `⦋m⦌ ⊗ ⦋n⦌ = ⦋m + n + 1⦌`, provides `inl` and `inr` morphisms for tensor product decomposition, and proves pentagon and associator properties |

## Subdirectories

No subdirectories.

## Search Tags

augmented-simplex-category initial-object monoidal-category tensor-product ordinal-sum augmented-simplicial-objects augmented-cosimplicial-objects with-initial associator unitor inl-inr categorical-equivalence
