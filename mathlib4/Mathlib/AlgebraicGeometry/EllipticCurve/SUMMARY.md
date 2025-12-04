---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/EllipticCurve
generated: 2025-12-04T23:15:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 10
subdirs_count: 4
---

# EllipticCurve

## Overview

The `EllipticCurve/` directory provides a comprehensive formalization of elliptic curves in Lean4, encompassing both the classical algebraic theory and multiple computational coordinate systems. At its foundation, the directory defines elliptic curves as nonsingular Weierstrass curves given by equations of the form `Y² + a₁XY + a₃Y = X³ + a₂X² + a₄X + a₆`, develops the theory of variable changes and isomorphisms, establishes various normal forms for elliptic curves over different characteristics (2, 3, and otherwise), and constructs explicit models with prescribed j-invariants.

The directory provides three complete, equivalent coordinate representations, each with full group law implementations: (1) **Affine coordinates** establish the fundamental group structure via the secant-and-tangent process, connecting to the ideal class group of the coordinate ring; (2) **Projective coordinates** include the point at infinity as a proper projective point using homogeneous equations, avoiding special case handling; (3) **Jacobian coordinates** use weighted projective coordinates `(2, 3, 1)` to enable efficient cryptographic implementations by eliminating field inversions in point arithmetic. All three coordinate systems are proven equivalent via explicit isomorphisms.

Beyond coordinate representations, the directory includes reduction theory for elliptic curves over discrete valuation rings (minimal Weierstrass equations and good reduction), and the theory of **division polynomials**—polynomials whose roots are the x-coordinates of n-torsion points. Together, these components provide a complete foundation for both theoretical investigations and practical applications in cryptography and number theory.

## Key Files

| File | Purpose |
|------|---------|
| Weierstrass.lean | Defines the fundamental `WeierstrassCurve` structure with coefficients `a₁, a₂, a₃, a₄, a₆`, computes standard quantities (b₂, b₄, b₆, b₈, c₄, c₆), defines the discriminant Δ and the `IsElliptic` typeclass (asserting Δ is a unit), defines the j-invariant, and establishes formulas in characteristic 2 and 3 |
| VariableChange.lean | Defines admissible linear change of variables `(u, r, s, t)` corresponding to coordinate transformations `(X, Y) ↦ (u²X + r, u³Y + u²sX + t)`, establishes that variable changes form a group acting on Weierstrass curves, and proves the j-invariant is invariant under variable changes |
| NormalForms.lean | Defines type classes for various normal forms of Weierstrass equations based on field characteristic: `IsCharNeTwoNF` (characteristic ≠ 2), `IsShortNF` (characteristic ≠ 2 or 3, or char 3 with j=0), `IsCharThreeNF` and `IsCharThreeJNeZeroNF` (characteristic 3), `IsCharTwoNF`, `IsCharTwoJNeZeroNF`, and `IsCharTwoJEqZeroNF` (characteristic 2), with explicit transformations to each normal form |
| ModelsWithJ.lean | Constructs explicit Weierstrass curves with prescribed j-invariants: `ofJ0` gives `Y² + Y = X³` (j=0), `ofJ1728` gives `Y² = X³ + X` (j=1728), `ofJNe0Or1728` gives a curve with arbitrary j-invariant, and `ofJ` combines these to construct an elliptic curve for any j |
| IsomOfJ.lean | Proves that elliptic curves with the same j-invariant over a separably closed field are isomorphic, by showing the existence of a variable change transforming one into the other, handling all characteristic cases separately |
| Reduction.lean | Defines reduction theory for elliptic curves over discrete valuation rings and local fields: `IsIntegral` predicate for curves with integral coefficients, `IsMinimal` for minimal Weierstrass equations (minimal discriminant valuation), `reduction` map to the residue field, and `IsGoodReduction` predicate |
| Group.lean | **Deprecated** (2025-05-07): Import module for affine curve point group structure, now superseded by `Affine/Point.lean` which provides the complete group structure implementation |
| Affine.lean | **Deprecated** (2025-05-03): Import module for affine coordinate theory, now superseded by the `Affine/` subdirectory with separate modules for basic definitions, formulas, and point structure |

## Subdirectories

- [x] `Affine/` - Affine coordinate formalization with complete group law via secant-and-tangent process, Weierstrass polynomial and nonsingular conditions, explicit negation and addition formulas, and injective group homomorphism to the ideal class group of the coordinate ring F[X,Y]/⟨W(X,Y)⟩ (3 files)
- [x] `Jacobian/` - Weighted projective coordinates `[x : y : z]` with weights `(2, 3, 1)` for cryptographically efficient point arithmetic; provides `(2, 3, 1)`-homogeneous Weierstrass equation, inversion-free doubling and addition formulas, and group isomorphism `toAffineAddEquiv` to affine points (3 files)
- [x] `Projective/` - Standard projective coordinates `[x : y : z]` including point at infinity `[0 : 1 : 0]`; establishes homogeneous Weierstrass equation, partial derivative nonsingular conditions, degree-4 homogeneous group operation formulas, and abelian group structure isomorphic to affine points (3 files)
- [x] `DivisionPolynomial/` - Division polynomials as normalized elliptic divisibility sequences (EDS), both univariate (`preΨₙ`, `ΨSqₙ`, `Φₙ`) and bivariate (`ψₙ`, `φₙ`) forms; includes recursive definitions, degree formulas (`deg(preΨₙ) = (n²-4)/2` for even n, `(n²-1)/2` for odd n), and leading coefficient calculations (2 files)

## Search Tags

elliptic-curves weierstrass-equations weierstrass-polynomial j-invariant discriminant variable-change normal-forms characteristic-2 characteristic-3 isomorphisms reduction discrete-valuation-ring minimal-weierstrass good-reduction affine-coordinates jacobian-coordinates projective-coordinates weighted-projective homogeneous-polynomial homogeneous-equation division-polynomials elliptic-divisibility-sequences torsion-points group-law abelian-group point-addition point-doubling negation-formula slope-formula secant-tangent-process nonsingular-condition partial-derivatives point-at-infinity coordinate-ring ideal-class-group fractional-ideals cryptographic-efficiency field-inversion-avoidance base-change polynomial-degree leading-coefficients number-theory
