---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Spectrum
generated: 2026-02-01T23:50:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 0
subdirs_count: 2
---

# Spectrum

## Overview

The `Spectrum/` directory provides a comprehensive formalization of the prime spectrum (Spec R) and maximal spectrum (mSpec R) of commutative rings, which are fundamental objects in algebraic geometry and scheme theory. The prime spectrum, consisting of all prime ideals with the Zariski topology, is developed extensively with full functoriality (comap operations for ring homomorphisms), topological properties (spectral space structure, Noetherian/Jacobson space results), constructible sets, Chevalley's theorem on images under finite presentation morphisms, and specialized results for polynomial rings, tensor products, and module support. The maximal spectrum embeds naturally as a subspace of the prime spectrum and includes localization theory establishing the injectivity of canonical maps to products of localizations. Together these provide the foundational infrastructure for scheme theory in mathlib4, with 16 files on prime spectra covering everything from basic definitions to deep results like Chevalley's theorem, and 4 files on maximal spectra covering their topology and localization properties.

## Key Files

No files directly in this directory - all content is organized in subdirectories.

## Subdirectories

- [x] `Prime/` - Prime spectrum Spec R with 16 files: core definitions, Zariski topology and spectral space structure, functoriality via comap, constructible sets and Chevalley's theorem, specialized results for polynomial rings, Jacobson/Noetherian rings, tensor products, module support, and free locus
- [x] `Maximal/` - Maximal spectrum mSpec R with 4 files: definitions, basic properties, subspace topology from prime spectrum, localization theory including injectivity of toPiLocalization map

## Search Tags

prime-spectrum Spec maximal-spectrum mSpec Zariski-topology prime-ideal maximal-ideal spectral-space algebraic-geometry scheme-theory zero-locus basic-open vanishing-ideal comap functoriality localization constructible-set Chevalley-theorem finite-presentation Jacobson-space Noetherian-space Artinian-ring polynomial-ring tensor-product module-support free-locus going-down universal-homeomorphism subspace-topology T1-space toPiLocalization Krull-dimension minimal-prime closed-point irreducible-component
