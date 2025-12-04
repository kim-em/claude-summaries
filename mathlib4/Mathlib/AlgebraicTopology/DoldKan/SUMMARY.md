---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/DoldKan
generated: 2025-12-04T00:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 19
subdirs_count: 0
---

# DoldKan

## Overview

The `DoldKan/` directory contains a complete formalization of the Dold-Kan correspondence, a fundamental equivalence in homological algebra stating that for any abelian (or more generally pseudoabelian) category C, there is an equivalence of categories between simplicial objects in C and chain complexes in C (indexed by ℕ with homological grading). The implementation uses an innovative approach via idempotent completions (Karoubi envelopes) to construct the equivalence first for pseudoabelian categories, then specializes to abelian categories. The key technical innovation is the construction of a projection endomorphism PInfty that identifies the normalized Moore complex as a formal direct factor of the alternating face map complex, avoiding the need to work with kernel subobjects directly.

## Key Files

| File | Purpose |
|------|---------|
| Equivalence.lean | Main entry point defining the Dold-Kan equivalence `SimplicialObject A ≌ ChainComplex A ℕ` for abelian categories, with detailed documentation of the overall proof strategy and construction pipeline |
| EquivalencePseudoabelian.lean | Dold-Kan equivalence for pseudoabelian (idempotent complete) categories, obtained by composing the Karoubi envelope equivalence with toKaroubi equivalences |
| EquivalenceAdditive.lean | Intermediate equivalence `Karoubi (SimplicialObject C) ≌ Karoubi (ChainComplex C ℕ)` for additive categories, the foundation for both pseudoabelian and abelian cases |
| FunctorN.lean | Constructs functors N₁: SimplicialObject C ⥤ Karoubi (ChainComplex C ℕ) and N₂: Karoubi (SimplicialObject C) ⥤ Karoubi (ChainComplex C ℕ) using PInfty as a formal direct factor |
| FunctorGamma.lean | Constructs the inverse functor Γ₀: ChainComplex C ℕ ⥤ SimplicialObject C using coproduct decompositions indexed by epi-mono factorizations, and its extension Γ₂ to Karoubi envelopes |
| PInfty.lean | Defines the idempotent projection PInfty: K[X] ⟶ K[X] by taking limits of projections P q; this endomorphism corresponds to projection onto the normalized Moore subcomplex |
| Projections.lean | Constructs the sequence of projections P q: K[X] ⟶ K[X] inductively, ensuring q higher face maps vanish on the image; foundation for PInfty construction |
| Homotopies.lean | Defines null homotopic maps Hσ q: K[X] ⟶ K[X] used to construct projections P q by altering the identity endomorphism, ensuring P q are automatically chain complex morphisms homotopic to identity |
| Faces.lean | Technical lemmas about vanishing of face maps on images of projections, crucial for verifying that PInfty projects onto the normalized subcomplex |
| Degeneracies.lean | Shows PInfty vanishes on images of degeneracy operators, key property for constructing the isomorphism N₂Γ₂: Γ₂ ⋙ N₂ ≅ 𝟭 (Karoubi (ChainComplex C ℕ)) |
| Decomposition.lean | Proves decomposition of identity X _⦋n⦌ ≅ PInfty.f n ⊕ (degeneracies), used to show N₂ reflects isomorphisms |
| NReflectsIso.lean | Proves N₁ and N₂ reflect isomorphisms using the decomposition results; critical for showing Γ₂N₂.trans is an isomorphism |
| NCompGamma.lean | Constructs natural transformation Γ₂N₂.trans: N₂ ⋙ Γ₂ ⟶ 𝟭 (Karoubi (SimplicialObject C)) and proves it's an isomorphism |
| GammaCompN.lean | Constructs the isomorphism N₂Γ₂: Γ₂ ⋙ N₂ ≅ 𝟭 (Karoubi (ChainComplex C ℕ)) using the vanishing property on degeneracies |
| Normalized.lean | For abelian categories, proves N₁ is isomorphic to normalizedMooreComplex A ⋙ toKaroubi, connecting the formal direct factor construction to the classical normalized Moore complex |
| Compatibility.lean | General framework for changing functors and inverses in equivalences while preserving definitional properties; used to ensure the final equivalence has normalizedMooreComplex as its functor and Γ₀ as inverse |
| SplitSimplicialObject.lean | For split simplicial objects, defines nondegComplex functor extracting the chain complex of nondegenerate simplices, and proves it's isomorphic to N₁ |
| HomotopyEquivalence.lean | Shows the inclusion of normalized Moore complex into alternating face map complex is a homotopy equivalence (using PInfty as the retraction) |
| Notations.lean | Defines notation K[X] for alternatingFaceMapComplex.obj X and N[X] for normalizedMooreComplex.obj X |

## Subdirectories

None - this is a leaf directory containing only implementation files.

## Search Tags

dold-kan correspondence equivalence simplicial-objects chain-complexes normalized-moore-complex alternating-face-map-complex idempotent-completion karoubi-envelope pseudoabelian abelian-category homological-algebra projection-endomorphism PInfty direct-factor homotopy-equivalence degeneracies face-maps functoriality split-simplicial-object category-theory
