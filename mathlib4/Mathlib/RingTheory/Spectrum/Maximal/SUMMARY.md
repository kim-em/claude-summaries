---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Spectrum/Maximal
generated: 2026-02-01T23:45:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Maximal

## Overview

The `Maximal/` directory contains the formalization of the maximal spectrum (mSpec R) of a commutative (semi)ring. The maximal spectrum is the type of all maximal ideals, naturally embedded as a subset of the prime spectrum with the subspace topology. This directory provides the core definitions, basic properties, topological structure, and localization theory for maximal spectra, including fundamental results like the injectivity of the canonical map to products of localizations and finiteness results.

## Key Files

| File | Purpose |
|------|---------|
| `Defs.lean` | Core definition of `MaximalSpectrum R` as a structure wrapping a maximal ideal |
| `Basic.lean` | Basic properties: equivalence with subtype, injection into prime spectrum, nonemptiness for nontrivial rings |
| `Topology.lean` | Zariski topology on maximal spectrum as subspace topology from prime spectrum, T1 space instance, continuity of inclusion |
| `Localization.lean` | Localization theory: intersection of localizations equals the ring, `toPiLocalization` map (always injective), functoriality, finiteness results for surjective cases |

## Subdirectories

(None - this is a leaf directory)

## Search Tags

maximal-spectrum mSpec maximal-ideal Zariski-topology subspace-topology T1-space localization product-of-localizations toPiLocalization intersection-of-localizations finiteness-results integral-domain fraction-ring Krull-dimension algebraic-geometry commutative-algebra
