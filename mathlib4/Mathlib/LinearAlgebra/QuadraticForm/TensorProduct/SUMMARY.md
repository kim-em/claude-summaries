---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/QuadraticForm/TensorProduct
generated: 2026-01-25T23:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# TensorProduct

## Overview

The `TensorProduct/` subdirectory provides isometry and isometric equivalence structures for tensor products of quadratic forms. It establishes that standard tensor product operations (commutativity, associativity, identity maps) preserve quadratic form structure, extending the basic `QuadraticForm.tmul` construction from the parent directory with categorical coherence properties. All results require `Invertible (2 : R)` to ensure the correspondence between quadratic forms and their associated symmetric bilinear forms.

## Key Files

| File | Purpose |
|------|---------|
| Isometries.lean | Tensor product isometries and coherence isomorphisms: `Isometry.tmul` (functorial `TensorProduct.map` for isometries), `tensorComm` (commutativity `Q₁.tmul Q₂ ≅ Q₂.tmul Q₁` via `TensorProduct.comm`), `tensorAssoc` (associativity `(Q₁.tmul Q₂).tmul Q₃ ≅ Q₁.tmul (Q₂.tmul Q₃)` via `TensorProduct.assoc`), `tensorRId` (right identity `Q.tmul sq ≅ Q` via `TensorProduct.rid`), and `tensorLId` (left identity `sq.tmul Q ≅ Q` via `TensorProduct.lid`) - split from main TensorProduct.lean for compilation performance |

## Subdirectories

None

## Search Tags

tensor-products quadratic-forms isometry isometric-equivalence tensor-coherence commutativity associativity identity-maps functoriality monoidal-structure invertible-2
