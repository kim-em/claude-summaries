---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/EllipticCurve/Jacobian
generated: 2025-12-04T12:46:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Jacobian

## Overview

The `Jacobian/` subdirectory implements the Jacobian coordinate system for elliptic curves, providing an efficient representation that avoids field inversions in point arithmetic. Jacobian coordinates use weighted projective coordinates `[x : y : z]` with weights `(2, 3, 1)`, where points are equivalent under scaling by units: `(x, y, z) ∼ (u²x, u³y, uz)`. This representation satisfies the `(2, 3, 1)`-homogeneous Weierstrass equation `Y² + a₁XYZ + a₃YZ³ = X³ + a₂X²Z² + a₄XZ⁴ + a₆Z⁶`. The directory establishes the complete group structure on nonsingular Jacobian points and proves equivalence with the affine point group via the `toAffineAddEquiv` isomorphism.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the fundamental structure of Jacobian coordinates: the `PointClass` equivalence type for weighted projective points, the `(2, 3, 1)`-homogeneous Weierstrass polynomial and its partial derivatives, the `Nonsingular` predicate requiring non-vanishing of some partial derivative, and lemmas establishing the relationship between Jacobian and affine coordinates via the map `(x, y, z) ↦ (x/z², y/z³)` when `z ≠ 0` (27KB, 582 lines) |
| Formula.lean | Provides explicit polynomial formulae for group operations in Jacobian coordinates: `negY` for negation, `dblZ/dblX/dblY` for point doubling, and `addZ/addX/addY` for point addition, where all operations are `(2, 3, 1)`-homogeneous and avoid field divisions by working with polynomial expressions (designed to minimize inversions in cryptographic implementations), with proofs relating these formulae to the corresponding affine operations when converted via dehomogenization (40KB, 826 lines) |
| Point.lean | Defines the type `Jacobian.Point` of nonsingular Jacobian points as equivalence classes with the nonsingular condition, implements the group operations (negation, addition) using the formulae from `Formula.lean`, proves `nonsingular_neg` and `nonsingular_add` showing group operations preserve nonsingularity, constructs the addition-preserving equivalence `toAffineAddEquiv : W.Point ≃+ W.toAffine.Point` between Jacobian and affine points, and derives the `AddCommGroup` instance for `Jacobian.Point` by transporting the group structure from affine coordinates (31KB, 646 lines) |

## Subdirectories

None

## Search Tags

elliptic-curves jacobian-coordinates weighted-projective group-law point-addition point-doubling nonsingular homogeneous-polynomial partial-derivatives equivalence-class affine-correspondence cryptographic-efficiency field-inversion-avoidance weierstrass-equation point-arithmetic
