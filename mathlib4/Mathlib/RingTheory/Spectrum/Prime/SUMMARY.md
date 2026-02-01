---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Spectrum/Prime
generated: 2026-02-01T22:45:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 16
subdirs_count: 0
---

# Prime

## Overview

The `Prime/` directory contains the comprehensive formalization of the prime spectrum (Spec R) of commutative semirings and rings. It defines the prime spectrum as the type of all prime ideals, establishes the Zariski topology, proves fundamental topological properties (spectral space structure, Noetherian space when R is Noetherian), and develops the functoriality of the spectrum construction. This includes comap operations induced by ring homomorphisms, constructible sets, Chevalley's theorem on images under finite presentation morphisms, and specialized results for polynomial rings, Jacobson rings, Noetherian rings, and tensor products.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `PrimeSpectrum R` as a structure containing a prime ideal, with the specialization partial order |
| Basic.lean | Fundamental properties: zero locus, vanishing ideal, correspondence between prime spectra and prime ideals, product spectra |
| Topology.lean | Zariski topology construction, basic opens, spectral space instance, localization embeddings, closed/irreducible set characterizations (64KB, 100+ results) |
| RingHom.lean | Functoriality: `comap` operation for ring homomorphisms, continuity, fiber properties, localization behavior |
| Polynomial.lean | Prime spectrum of polynomial rings `R[X]` and `R[X̲]`, open map property of `Spec R[X] → Spec R`, nilpotency criteria via characteristic polynomials |
| ConstructibleSet.lean | Machinery for constructible sets: `BasicConstructibleSetData`, `ConstructibleSetData`, operations on constructible sets |
| Chevalley.lean | **Chevalley's theorem**: finite presentation morphisms preserve constructible sets, going-down property implies open maps |
| ChevalleyComplexity.lean | Technical proof of Chevalley's theorem using complexity arguments (910 lines) |
| Jacobson.lean | Prime spectrum of Jacobson rings is a Jacobson space, equivalence characterizations for Noetherian Jacobson rings |
| Noetherian.lean | Prime spectrum of Noetherian rings is a Noetherian space, Artinian rings have discrete spectrum and Krull dimension ≤ 0 |
| Homeomorph.lean | Universal homeomorphism properties: purely inseparable field extensions induce homeomorphisms on spectra |
| FreeLocus.lean | Free locus of a module: the set of primes where the localization is free, rank functions, locally constant rank for flat modules |
| IsOpenComapC.lean | The structure map `Spec R[X] → Spec R` is an open map (alternative proof using coefficient-based arguments) |
| LTSeries.lean | Lemmas about chains of prime ideals in Noetherian rings, including ability to find chains with specified membership properties |
| Module.lean | Module-theoretic subsets of prime spectra: support, closed support for finite modules, localization criteria |
| TensorProduct.lean | Prime spectrum of tensor products `S ⊗[R] T`, embedding into product `Spec S × Spec T` when R → T is surjective on stalks |

## Subdirectories

None - all content is in files.

## Search Tags

prime-spectrum Spec Zariski-topology prime-ideal spectral-space algebraic-geometry zero-locus basic-open vanishing-ideal comap functoriality localization constructible-set Chevalley-theorem finite-presentation Jacobson-space Noetherian-space Artinian-ring polynomial-ring tensor-product module-support free-locus going-down universal-homeomorphism purely-inseparable surjective-on-stalks Krull-dimension minimal-prime maximal-ideal closed-point irreducible-component
