---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/LocalRing/ResidueField
generated: 2026-02-01T19:45:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 6
subdirs_count: 0
---

# ResidueField

## Overview

The `ResidueField/` directory develops the theory of residue fields for local rings and prime ideals. For a local ring R with maximal ideal m, the residue field is k = R/m. For a prime ideal I in a commutative ring, the residue field κ(I) is the field of fractions of R/I (equivalently, the residue field of the localization at I). This includes functoriality (maps between residue fields from local homomorphisms), fiber theory (κ(p) ⊗ S characterizes the fiber of Spec S → Spec R over p), separability and algebraicity instances, and applications to polynomial algebras.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `IsLocalRing.ResidueField` as R/m for local rings, and `residue : R →+* ResidueField R` quotient map |
| Basic.lean | Properties of residue field for local rings: `lift` for descending local homomorphisms into fields, `map` for induced maps between residue fields, `mapEquiv` for ring isomorphisms, `MulSemiringAction` instances, finite-dimensionality results for algebra extensions |
| Ideal.lean | Residue field of arbitrary prime ideals: `Ideal.ResidueField I` := κ(Localization.AtPrime I); `IsFractionRing (R ⧸ I) I.ResidueField` instance; `lift` and `liftₐ` for factoring through residue fields; surjectivity on stalks |
| Fiber.lean | Fiber theory for ring maps: `Ideal.Fiber p S` := κ(p) ⊗ S; `PrimeSpectrum.preimageEquivFiber` showing the fiber of Spec S → Spec R at p is homeomorphic to Spec(κ(p) ⊗ S); order isomorphisms for primes lying over |
| Instances.lean | Automatic instances: separability transfers between (A/p, B/q) and (κ(p), κ(q)); algebraicity of residue fields over quotients and extensions |
| Polynomial.lean | Polynomial algebra applications: `residueFieldMapCAlgEquiv` showing κ(I[X]) ≃ₐ κ(I)(X); `fiberEquivQuotient` showing κ(p) ⊗ (R[X]/I) ≃ κ(p)[X]/I |

## Subdirectories

(none)

## Search Tags

residue-field local-ring maximal-ideal quotient-field prime-ideal localization fiber tensor-product spectrum PrimeSpectrum homeomorphism separable algebraic polynomial rational-function IsLocalRing ResidueField residue lift map IsFractionRing surjectiveOnStalks
