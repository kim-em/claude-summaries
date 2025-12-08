---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry
generated: 2025-12-04T23:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 28
subdirs_count: 7
---

# AlgebraicGeometry

## Overview

The `AlgebraicGeometry/` directory provides a comprehensive formalization of algebraic geometry in Lean4, centered on the theory of schemes and their applications. At its foundation, the directory establishes schemes as locally ringed spaces that are locally isomorphic to the spectrum of a commutative ring, constructs the fundamental Spec functor and its adjunction with the global sections functor Γ (the Γ ⊣ Spec adjunction), and develops the complete machinery for building complex schemes via gluing constructions and fiber products (pullbacks). The 28 core files provide essential infrastructure including the structure sheaf on prime spectra, the affine-scheme equivalence (AffineScheme ≌ CommRingᵒᵖ), limits and colimits in the category of schemes, open immersions and restriction to open subschemes, and specialized structures such as residue fields, function fields, stalks, rational maps, and valuative criteria for separation and properness.

The directory's seven subdirectories develop the complete theory of modern algebraic geometry: (1) **Morphisms/** provides a comprehensive framework for 30+ morphism properties (affine, closed immersions, étale, finite, flat, proper, separated, smooth, and universal properties) with systematic local-to-global principles via the `IsZariskiLocalAtTarget/Source` infrastructure; (2) **EllipticCurve/** formalizes elliptic curves with three equivalent coordinate systems (affine, projective, Jacobian), complete group law implementations, normal forms for all characteristics, explicit models for prescribed j-invariants, reduction theory for discrete valuation rings, and division polynomials for torsion point computation; (3) **ProjectiveSpectrum/** constructs the Proj functor for graded rings with proofs that Proj is a proper and separated scheme over Spec A₀; (4) **Cover/** develops the theory of covers with respect to morphism properties, including open covers, affine covers, locally directed covers with transition maps, and covers over a base scheme; (5) **Sites/** formalizes Grothendieck topologies (Zariski, étale) as the categorical framework for sheaf theory and descent, proving subcanonicity and establishing equivalences between sheaf categories; (6) **IdealSheaf/** constructs closed subschemes via ideal sheaves with functorial operations (pullback/pushforward), scheme-theoretic images, and the kernel adjunction; (7) **Modules/** establishes the abelian category X.Modules of sheaves of modules and the tilde construction M^~ with stalk isomorphisms (M^~)_x ≅ M_x.

Together, these components provide the complete foundation for modern algebraic geometry in Lean4, supporting both theoretical investigations (cohomology, descent theory) and practical applications (elliptic curve cryptography, computational number theory), with rigorous categorical infrastructure and geometric intuition preserved throughout.

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

- [x] `Morphisms/` - Comprehensive theory of morphism properties (30 files including affine, closed immersions, étale, finite, flat, integral, proper, quasi-compact, separated, smooth, and universal properties)
- [x] `EllipticCurve/` - Elliptic curves over fields and rings, including Weierstrass forms, group structure, Jacobian coordinates, normal forms, projective and affine models, division polynomials, and reduction theory
- [x] `ProjectiveSpectrum/` - Projective spectrum Proj of graded rings, the projective analogue of Spec for graded commutative algebras
- [x] `Cover/` - Theory of covers of schemes with respect to morphism properties, open covers, locally directed covers with transition maps, covers over a base, and functorial operations
- [x] `Sites/` - Grothendieck sites and topologies on schemes (Zariski, étale, etc.) for sheaf theory and descent
- [x] `IdealSheaf/` - Theory of ideal sheaves on schemes, including the IdealSheafData structure, closed subscheme construction via gluing, functorial operations (pullback/pushforward), and scheme-theoretic images
- [x] `Modules/` - Theory of sheaves of modules over schemes, abelian category X.Modules, and the tilde construction M^~ from R-modules to sheaves with stalk isomorphisms

## Search Tags

algebraic-geometry schemes spec functor structure-sheaf affine-schemes morphisms pullbacks gluing limits colimits locally-ringed-spaces adjunction gamma-spec elliptic-curves rational-maps open-immersion projective-spectrum sheaves modules ideal-sheaf grothendieck-topology sites covers categorical-limits fiber-products quasi-coherent separation properness smoothness flatness
