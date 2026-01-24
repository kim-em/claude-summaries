---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/VectorField
generated: 2026-01-24T07:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# VectorField

## Overview

The `VectorField/` directory formalizes vector fields on smooth manifolds and their key operations. Vector fields are represented as dependent functions `V : (x : M) -> TangentSpace I x` assigning a tangent vector to each point. The library defines the pullback of vector fields under smooth maps (using the inverse of the manifold derivative) and the Lie bracket of two vector fields (defined via pullback through extended charts). Key results include that the pullback preserves Lie brackets (`mpullback_mlieBracket`) and the Leibniz/Jacobi identity for Lie brackets.

## Key Files

| File | Purpose |
|------|---------|
| Pullback.lean | Defines the pullback of vector fields under maps between manifolds (`mpullback`, `mpullbackWithin`). The pullback uses the inverse of the manifold derivative, with junk value zero when the derivative is not invertible. Proves regularity results: pullback of a `C^m` vector field by a `C^n` map (with `m+1 <= n` and invertible derivative) is `C^m`. Requires `CompleteSpace E` to ensure the set of invertible linear maps is open. |
| LieBracket.lean | Defines the Lie bracket of two vector fields on a manifold (`mlieBracket`, `mlieBracketWithin`). The Lie bracket is computed by pulling back to the model space via extended charts, computing the vector space Lie bracket there, and pulling back the result. Proves the Leibniz/Jacobi identity `[U, [V, W]] = [[U, V], W] + [V, [U, W]]`, that pullback preserves Lie brackets, and smoothness of the Lie bracket operation. |

## Subdirectories

(none)

## Search Tags

vector-field lie-bracket pullback manifold tangent-space mlieBracket mpullback jacobi-identity leibniz-identity contmdiff mdifferentiable smooth-vector-field vector-field-bracket
