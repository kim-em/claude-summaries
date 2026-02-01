---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/RingHom
generated: 2026-02-01T19:45:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 18
subdirs_count: 0
---

# RingHom

## Overview

The `RingHom/` directory contains meta-property theory for ring homomorphisms in commutative algebra. Each file establishes fundamental categorical and local properties (stability under composition, base change, localization preservation, etc.) for a specific class of ring homomorphisms. These properties are essential for algebraic geometry, where morphisms of schemes are studied locally via their induced ring homomorphisms. The directory provides the algebraic foundation for concepts like finite morphisms, flat morphisms, smooth morphisms, and étale morphisms.

## Key Files

| File | Purpose |
|------|---------|
| Finite.lean | Finite ring homomorphisms (module-finite); proves localization preservation, stability under base change, and gluability from open covers |
| FiniteType.lean | Finitely generated algebras (finite type); establishes locality, localization preservation, and characterization via spanning sets |
| FinitePresentation.lean | Finitely presented ring homomorphisms; proves locality and stability properties using quotients of polynomial rings |
| Flat.lean | Flat ring homomorphisms preserving exactness; shows locality, base change stability, going-down property, and prime spectrum generalization |
| FaithfullyFlat.lean | Faithfully flat ring homomorphisms (flat + surjective on spectra); proves composition stability and base change preservation |
| Smooth.lean | Smooth ring homomorphisms (formally smooth + finitely presented); establishes locality via smooth locus techniques |
| FormallySmooth.lean | Formally smooth homomorphisms via Algebra.FormallySmooth; proves stability and localization properties (defined via smooth locus, not repeated here) |
| Unramified.lean | Formally unramified ring homomorphisms (trivial Kähler differentials); proves locality using unramified locus |
| Etale.lean | Étale ring homomorphisms (formally unramified + smooth); shows meta properties via conjunction of component properties |
| StandardSmooth.lean | Standard smooth ring homomorphisms from polynomial algebras; defines relative dimension and proves composition properties |
| LocallyStandardSmooth.lean | Locally standard smooth ring homomorphisms (standard smooth on open cover); shorter variant focusing on local characterization |
| Integral.lean | Integral ring homomorphisms (all elements integral); proves stability under composition, base change, and localization glueing |
| QuasiFinite.lean | Quasi-finite ring homomorphisms (finite fibers over primes); establishes locality and characterization via integral + finite type |
| Bijective.lean | Bijective ring homomorphisms; shows stability under composition, base change, and gluability from localizations |
| Injective.lean | Injective ring homomorphisms; proves stability under composition and respects isomorphisms |
| Surjective.lean | Surjective ring homomorphisms; establishes localization preservation, base change stability, and gluability |
| OpenImmersion.lean | Open immersion ring homomorphisms (standard opens in spectrum); defines IsStandardOpenImmersion property (content not fully examined) |
| EssFiniteType.lean | Essentially finite type ring homomorphisms (finite type modulo nilradical); recent addition for refined finiteness conditions (content not fully examined) |
| Locally.lean | Target-local closure construction for arbitrary ring homomorphism properties; proves that Locally P inherits stability properties from P and is always local on target |

## Subdirectories

(No subdirectories)

## Search Tags

ring-homomorphism meta-properties finite finite-type finite-presentation flat faithfully-flat smooth formally-smooth etale unramified integral quasi-finite bijective injective surjective localization base-change composition stability locality open-cover glueing property-is-local localization-preserves respects-iso standard-smooth Kähler-differentials formally-unramified algebraic-geometry scheme-morphisms local-properties target-local source-local
