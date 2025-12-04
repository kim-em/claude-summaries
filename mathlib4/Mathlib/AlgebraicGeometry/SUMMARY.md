---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry
generated: 2025-12-04T04:09:11Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 28
subdirs_count: 7
---

# AlgebraicGeometry

## Overview

The `AlgebraicGeometry/` directory provides a comprehensive formalization of algebraic geometry in Lean4, centered on the theory of schemes. It defines schemes as locally ringed spaces that are locally isomorphic to the spectrum of a commutative ring, establishes the fundamental Spec functor and its adjunction with the global sections functor Γ, and develops the theory of morphisms between schemes (including affine, étale, proper, separated, smooth morphisms and many other properties). The directory includes specialized theories for elliptic curves, rational maps, gluing constructions, fiber products (pullbacks), and the projective spectrum, providing the categorical and geometric foundations for modern algebraic geometry.

## Key Files

| File | Purpose |
|------|---------|
| Scheme.lean | Defines the category of schemes as locally ringed spaces with local affine charts, including morphisms, categorical structure, and the fundamental isomorphism between schemes and locally ringed spaces locally isomorphic to Spec R |
| Spec.lean | Defines the Spec functor from commutative rings to locally ringed spaces in three stages (topological spaces, sheafed spaces, locally ringed spaces), providing the fundamental construction mapping rings to geometric objects |
| StructureSheaf.lean | Constructs the structure sheaf on the prime spectrum of a commutative ring as a subsheaf of localizations, with ring structure and basic isomorphisms (stalk isomorphisms and basic open isomorphisms) |
| AffineScheme.lean | Defines the category of affine schemes as the essential image of Spec, the IsAffine predicate for schemes, the canonical isomorphism X ≅ Spec Γ(X) for affine schemes, and the equivalence AffineScheme ≌ CommRingᵒᵖ |
| GammaSpecAdjunction.lean | Establishes the adjunction Γ ⊣ Spec between the global sections functor and the spectrum functor, the fundamental adjunction of algebraic geometry connecting rings and geometric spaces |
| Pullbacks.lean | Constructs fibered products (pullbacks) of schemes via gluing, showing that for an open cover {Uᵢ} of X, if fibered products Uᵢ ×[Z] Y exist, then X ×[Z] Y exists, reducing to the affine case |
| Gluing.lean | Provides the gluing construction for schemes: given a family of schemes with gluing data on overlaps, constructs the glued scheme as a multicoequalizer with canonical open immersions ι i : U i ⟶ glued |
| Limits.lean | Constructs various limits and colimits in the category of schemes: fibered products, terminal object (Spec ℤ), initial object (empty scheme), and coproducts (disjoint unions) |
| OpenImmersion.lean | Theory of open immersions between schemes, a fundamental class of morphisms that are locally isomorphisms onto open subschemes |
| RationalMap.lean | Defines partial maps (morphisms defined on dense open subschemes), equivalence of partial maps, and rational maps as equivalence classes, with correspondence to morphisms from Spec K(X) for integral schemes |
| Restrict.lean | Theory of restricting schemes to open subsets, providing the fundamental operation of passing to open subschemes |
| Over.lean | Schemes over a base scheme S, the foundation for relative algebraic geometry |
| Properties.lean | General properties of schemes and morphisms including various local and global geometric conditions |
| Stalk.lean | Stalks of the structure sheaf, the local rings at points of a scheme |
| ResidueField.lean | Residue fields at points of schemes, defined as the residue field of the local ring at that point |
| FunctionField.lean | Function fields of integral schemes, the field of rational functions on an irreducible variety |
| Noetherian.lean | Noetherian schemes, schemes with a finite affine open cover where each coordinate ring is Noetherian |
| QuasiAffine.lean | Quasi-affine schemes, schemes that can be embedded as dense open subschemes of affine schemes |
| Fiber.lean | Fibers of morphisms between schemes over a base |
| PointsPi.lean | Pi-points of schemes, generalizing the notion of points |
| SpreadingOut.lean | Spreading out techniques for extending morphisms and properties from generic points to open neighborhoods |
| ValuativeCriterion.lean | Valuative criteria for separation and properness of morphisms |
| AffineSpace.lean | Affine space as a scheme, the fundamental affine varieties |
| AffineTransitionLimit.lean | Limits in the category of affine schemes computed via transitions |
| GluingOneHypercover.lean | Gluing schemes using hypercovers, an advanced gluing technique |
| PullbackCarrier.lean | Carrier sets for pullback constructions |
| LimitsOver.lean | Limits in categories of schemes over a base |
| IdealSheaf.lean | Import file for the ideal sheaf theory subdirectory |

## Subdirectories

- [x] `Morphisms/` - Comprehensive theory of morphism properties (30 files including affine, closed immersions, étale, finite, flat, integral, proper, quasi-compact, separated, smooth, and universal properties) (complete)
- [x] `EllipticCurve/` - Elliptic curves over fields and rings, including Weierstrass forms, group structure, Jacobian coordinates, normal forms, projective and affine models, division polynomials, and reduction theory (complete)
- [x] `ProjectiveSpectrum/` - Projective spectrum Proj of graded rings, the projective analogue of Spec for graded commutative algebras (complete)
- [x] `Cover/` - Theory of covers of schemes with respect to morphism properties, open covers, locally directed covers with transition maps, covers over a base, and functorial operations (complete)
- [ ] `Sites/` - Grothendieck sites and topologies on schemes (Zariski, étale, etc.) for sheaf theory and descent (pending)
- [ ] `IdealSheaf/` - Theory of ideal sheaves and sheaves of ideals on schemes (pending)
- [ ] `Modules/` - Theory of sheaves of modules on schemes, quasi-coherent sheaves, and module operations (pending)

## Search Tags

algebraic-geometry schemes spec functor structure-sheaf affine-schemes morphisms pullbacks gluing limits colimits locally-ringed-spaces adjunction gamma-spec elliptic-curves rational-maps open-immersion projective-spectrum sheaves modules ideal-sheaf grothendieck-topology sites covers categorical-limits fiber-products quasi-coherent separation properness smoothness flatness
