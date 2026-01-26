---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Flat/FaithfullyFlat
generated: 2026-01-26T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# FaithfullyFlat

## Overview

The `FaithfullyFlat/` directory contains the comprehensive theory of faithfully flat modules and algebras over commutative rings. A module M is faithfully flat if it is flat and IM ≠ M for all maximal ideals I. This includes the core definition, numerous equivalent characterizations (proper ideals, faithful tensoring, exact sequence reflection, zero-map detection), structural properties (stability under composition, base change, linear equivalence), and specialized results for algebras (descent properties, prime spectrum surjectivity, local ring characterizations). The theory demonstrates that faithfully flat modules preserve and reflect exactness, making tensoring a faithful operation that detects vanishing of modules and maps.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of faithfully flat modules (`Module.FaithfullyFlat`) with characterizations via proper ideals, faithful tensoring (N ≠ 0 ↔ N ⊗ M ≠ 0), exact sequence reflection (exact iff exact after tensoring), and zero map detection (f = 0 iff f ⊗ M = 0); proves R is faithfully flat over itself, free nontrivial modules are faithfully flat, and faithfully flat descends along composition |
| Algebra.lean | Algebra-specific characterizations: proves faithfully flat algebras satisfy ideal contraction (I = I.map.comap), induce surjective maps on prime spectra, and provides converse (flat + surjective spectrum map → faithfully flat); establishes that flat local algebras over local rings are faithfully flat; proves tensoring m ↦ 1 ⊗ m is injective |
| Descent.lean | Descent properties for ring homomorphisms under faithfully flat base change: proves injectivity, surjectivity, and bijectivity of ring maps descend along faithfully flat extensions (if S ⊗ T → T is injective/surjective/bijective then R → T has same property) |

## Subdirectories

*(none)*

## Search Tags

faithfully-flat faithful-flatness flat-module tensor-product exact-sequence preservation reflection injective-map proper-ideal maximal-ideal faithful-functor zero-detection algebra prime-spectrum descent base-change composition free-module nontrivial local-ring ideal-contraction surjective-spectrum character-module faithful-smul linear-equivalence quotient-tensor equational-criterion stability
