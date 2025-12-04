---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/Morphisms
generated: 2025-12-04T04:13:13Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 30
subdirs_count: 0
---

# Morphisms

## Overview

The `Morphisms/` directory provides a comprehensive framework for defining and working with properties of morphisms between schemes in algebraic geometry. It establishes the foundational infrastructure for describing morphism properties that are local (at the source, target, or both), provides canonical constructions for deriving scheme morphism properties from ring homomorphism properties, and implements the full spectrum of standard geometric properties including affine, closed immersions, étale, finite, finite type, flat, integral, proper, quasi-compact, quasi-separated, separated, smooth, and various universal properties. This directory is central to the formalization of modern algebraic geometry, enabling precise characterization of morphisms through local-to-global principles.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core framework for morphism properties including `IsZariskiLocalAtTarget`, `IsZariskiLocalAtSource`, `AffineTargetMorphismProperty`, and `HasAffineProperty` type classes with API for working with properties local at the target or source |
| RingHomProperties.lean | Framework for defining scheme morphism properties from ring homomorphism properties via `affineLocally` and `targetAffineLocally` constructions, including `HasRingHomProperty` type class for properties local at both source and target |
| Affine.lean | Affine morphisms (preimages of affine opens are affine), with equivalence characterizations and stability under base change |
| AffineAnd.lean | Construction `targetAffineLocally (affineAnd P)` for properties requiring both affine preimages and ring hom property P |
| ClosedImmersion.lean | Closed immersions (closed embeddings with surjective stalk maps), the proper analog of closed subschemes |
| OpenImmersion.lean | Open immersions between schemes, morphisms that are locally isomorphisms onto open subschemes |
| Etale.lean | Étale morphisms (smooth of relative dimension zero) and the category `Scheme.Etale X` of schemes étale over X |
| Finite.lean | Finite morphisms (affine morphisms with finite ring maps), including stability under composition and base change |
| FiniteType.lean | Locally of finite type morphisms, where local rings are finitely generated algebras |
| FinitePresentation.lean | Locally of finite presentation morphisms, finitely presented algebras on affine opens |
| Flat.lean | Flat morphisms (flat stalk maps), equivalent to flatness of induced ring maps on affine opens |
| Smooth.lean | Smooth morphisms (locally standard smooth ring maps), with relative dimension variants |
| Integral.lean | Integral morphisms (affine with integral ring maps), morphisms that are affine and universally closed |
| Proper.lean | Proper morphisms (separated, universally closed, locally of finite type), the scheme-theoretic analog of compact maps |
| Separated.lean | Separated morphisms (diagonal is a closed immersion), the Hausdorff-like condition for schemes |
| QuasiCompact.lean | Quasi-compact morphisms (preimages of quasi-compact opens are quasi-compact), with characterization via spectral maps |
| QuasiSeparated.lean | Quasi-separated morphisms (diagonal is quasi-compact), weaker than separated |
| UniversallyClosed.lean | Universally closed morphisms (remain closed under base change), key component of properness |
| UniversallyOpen.lean | Universally open morphisms (remain open under base change) |
| UniversallyInjective.lean | Universally injective morphisms (remain injective under base change) |
| SurjectiveOnStalks.lean | Morphisms inducing surjective maps on all stalks, used in definition of closed immersions |
| Immersion.lean | Immersions (compositions of closed immersion with open immersion), locally closed embeddings |
| Preimmersion.lean | Preimmersions (homeomorphism onto image with surjective stalk maps), generalization of immersions |
| LocalIso.lean | Local isomorphisms, morphisms that are locally isomorphisms in the Zariski topology |
| IsIso.lean | Properties of isomorphisms of schemes |
| FormallyUnramified.lean | Formally unramified morphisms, infinitesimal lifting property related to separability |
| UnderlyingMap.lean | Properties of underlying continuous maps of scheme morphisms |
| LocalClosure.lean | Local closures of morphisms, technical tool for studying locally closed embeddings |
| Constructors.lean | Helper functions and constructors for building morphisms with specific properties |
| Descent.lean | Descent theory for morphism properties, studying when properties can be checked on covers |

## Subdirectories

(none)

## Search Tags

morphism-properties scheme-morphisms local-properties affine-morphisms closed-immersion open-immersion etale finite flat smooth proper separated quasi-compact quasi-separated integral universally-closed ring-hom-properties standard-smooth finite-type finite-presentation immersion categorical-properties base-change composition stability descent-theory diagonal-morphism zariski-local spectral-maps
