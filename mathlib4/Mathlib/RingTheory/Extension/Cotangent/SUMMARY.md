---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Extension/Cotangent
generated: 2026-01-26T09:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Cotangent

## Overview

The `Cotangent/` directory develops the naive cotangent complex theory for algebra presentations. The core construction associates a cotangent complex to a presentation `0 → I → R[x₁,...,xₙ] → S → 0`, yielding the sequence `I/I² → ⨁ᵢ S dxᵢ → Ω[S/R] → 0`. The theory includes: the cotangent space construction with canonical bases, exactness and surjectivity results, homotopy between presentation morphisms, the first homology H¹(L_{S/R}) independent of presentation choice, base change and localization behavior, and computational tools for showing presentations are submersive via Jacobian calculations from cotangent bases.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `CotangentSpace` (S ⊗[P.Ring] Ω[P.Ring⁄R]) and `cotangentComplex` (map I/I² → CotangentSpace); proves exactness `exact_cotangentComplex_toKaehler`; defines `H1Cotangent` (first homology of cotangent complex) and proves it is independent of presentation; includes base change formulas, morphism maps, and homotopy theory (Hom.Sub showing f-g induces homotopy); proves finite presentation when S is finitely presented over R |
| Basis.lean | Proves that free cotangent space I/I² can be realized via a presentation with kernel I' where I'/I'² is free on the images of relations; includes `exists_presentation_of_free_cotangent` constructing such presentations for finitely presented algebras; uses localization away construction and tensor product decompositions |
| Free.lean | Provides criteria for showing presentations are submersive based on cotangent bases; proves `cotangentRestrict_bijective` when H¹(L_{S/R}) = 0 and suitable basis conditions hold; includes `isUnit_jacobian_of_cotangentRestrict_bijective` showing pre-submersive presentations are submersive when cotangent restriction is bijective |
| LocalizationAway.lean | Studies cotangent behavior under localization away from an element; proves injectivity of T ⊗[S] (I/I²) → J/J² when T is localization of S; establishes splitting `cotangentCompLocalizationAwayEquiv`: J/J² ≃ T ⊗[S] (I/I²) × K/K² where K is kernel of localization presentation; includes section constructions and compatibility with Jacobi-Zariski sequence |

## Subdirectories

(none)

## Search Tags

cotangent-complex conormal-space kaehler-differentials presentation naive-cotangent-complex first-homology H1-cotangent exact-sequence base-change localization-away tensor-product generators kernel jacobian submersive homotopy finite-presentation free-module basis jacobi-zariski
