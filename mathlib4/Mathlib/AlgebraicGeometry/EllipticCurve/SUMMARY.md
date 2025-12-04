---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/EllipticCurve
generated: 2025-12-04T12:45:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 10
subdirs_count: 4
---

# EllipticCurve

## Overview

The `EllipticCurve/` directory provides a comprehensive formalization of elliptic curves in Lean4, focusing on the classical theory of Weierstrass curves. It defines elliptic curves as nonsingular Weierstrass curves given by equations of the form `Y² + a₁XY + a₃Y = X³ + a₂X² + a₄X + a₆`, develops the theory of variable changes and isomorphisms, establishes various normal forms for elliptic curves over different characteristics, and provides models with prescribed j-invariants. The directory includes specialized subdirectories for affine coordinates, Jacobian coordinates, projective coordinates, and division polynomials, providing both the algebraic foundations and computational representations of elliptic curves.

## Key Files

| File | Purpose |
|------|---------|
| Weierstrass.lean | Defines the fundamental `WeierstrassCurve` structure with coefficients `a₁, a₂, a₃, a₄, a₆`, computes standard quantities (b₂, b₄, b₆, b₈, c₄, c₆), defines the discriminant Δ and the `IsElliptic` typeclass (asserting Δ is a unit), defines the j-invariant, and establishes formulas in characteristic 2 and 3 |
| VariableChange.lean | Defines admissible linear change of variables `(u, r, s, t)` corresponding to coordinate transformations `(X, Y) ↦ (u²X + r, u³Y + u²sX + t)`, establishes that variable changes form a group acting on Weierstrass curves, and proves the j-invariant is invariant under variable changes |
| NormalForms.lean | Defines type classes for various normal forms of Weierstrass equations based on field characteristic: `IsCharNeTwoNF` (characteristic ≠ 2), `IsShortNF` (characteristic ≠ 2 or 3, or char 3 with j=0), `IsCharThreeNF` and `IsCharThreeJNeZeroNF` (characteristic 3), `IsCharTwoNF`, `IsCharTwoJNeZeroNF`, and `IsCharTwoJEqZeroNF` (characteristic 2), with explicit transformations to each normal form |
| ModelsWithJ.lean | Constructs explicit Weierstrass curves with prescribed j-invariants: `ofJ0` gives `Y² + Y = X³` (j=0), `ofJ1728` gives `Y² = X³ + X` (j=1728), `ofJNe0Or1728` gives a curve with arbitrary j-invariant, and `ofJ` combines these to construct an elliptic curve for any j |
| IsomOfJ.lean | Proves that elliptic curves with the same j-invariant over a separably closed field are isomorphic, by showing the existence of a variable change transforming one into the other, handling all characteristic cases separately |
| Reduction.lean | Defines reduction theory for elliptic curves over discrete valuation rings and local fields: `IsIntegral` predicate for curves with integral coefficients, `IsMinimal` for minimal Weierstrass equations (minimal discriminant valuation), `reduction` map to the residue field, and `IsGoodReduction` predicate |
| Group.lean | Import module for affine curve point group structure (deprecated as of 2025-05-07), now superseded by the Affine subdirectory |
| Affine.lean | Import module for affine coordinate theory (deprecated as of 2025-05-03), now superseded by the Affine subdirectory |

## Subdirectories

- [x] `Affine/` - Affine coordinate representation of elliptic curve points, including basic definitions, point arithmetic formulas, and group structure on the set of affine points (complete)
- [x] `Jacobian/` - Jacobian coordinate system for efficient elliptic curve arithmetic, avoiding inversions in field operations by using weighted projective coordinates `(2, 3, 1)` (complete)
- [x] `Projective/` - Projective coordinate representation of elliptic curve points, including the point at infinity as a proper projective point, with complete group law and equivalence to affine coordinates (complete)
- [x] `DivisionPolynomial/` - Division polynomials (polynomials whose roots are the x-coordinates of n-torsion points), including basic definitions and degree calculations (complete)

## Search Tags

elliptic-curves weierstrass-equations j-invariant discriminant variable-change normal-forms characteristic-2 characteristic-3 isomorphisms reduction discrete-valuation-ring minimal-weierstrass affine-coordinates jacobian-coordinates projective-coordinates division-polynomials torsion-points group-law
