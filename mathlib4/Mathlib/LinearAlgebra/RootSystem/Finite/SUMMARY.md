---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/RootSystem/Finite
generated: 2026-01-25T09:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Finite

## Overview

The `Finite/` directory contains theory specific to finite (finitely-indexed) root pairings. It establishes fundamental properties that arise when the index set is finite, including the canonical bilinear form construction, structural classification lemmas for crystallographic systems, nondegeneracy results, and the complete theory of the exceptional 𝔤₂ root system. Key achievements include proving Coxeter weights are bounded by 4, establishing positive-definiteness of the root form on the root span, and characterizing when sums/differences of roots remain roots based on pairing signs.

## Key Files

| File | Purpose |
|------|---------|
| CanonicalBilinear.lean | Canonical bilinear form on finite root pairings: Polarization (weight→coweight map summing coroot projections), RootForm (invariant bilinear form on weights), symmetry and Weyl-invariance, positive-semidefiniteness over ordered rings, root-positivity implying Coxeter weights ≤ 4, kernel characterizations, restricted forms over subrings (RootFormIn for S-valued pairings) |
| Lemmas.lean | Structural lemmas for finite crystallographic root pairings: Coxeter weights belong to {0,1,2,3,4}, complete enumeration of possible (pairing i j, pairing j i) pairs for crystallographic/reduced systems, root length comparison lemmas, closure under addition (negative pairing) and subtraction (positive pairing), orthogonality characterizations, invariant form implies root lengths related by factors of 2 or 3, dichotomy between systems with length ratios √2 vs √3 |
| Nondegenerate.lean | Nondegeneracy of canonical forms on finite root pairings: IsAnisotropic typeclass (no zero-length roots/coroots), positive-definiteness of RootForm on root span over ordered rings, equality of dimensions for root/coroot spans, injectivity of Polarization, nondegeneracy of restricted root form, IsBalanced instance for anisotropic pairings over fields, PolarizationEquiv as linear equivalence for root systems, linear independence equivalence between roots and coroots |
| G2.lean | Complete theory of 𝔤₂ root system: EmbeddedG2 typeclass (distinguished long/short roots pairing to -3), IsG2 and IsNotG2 characterizations, all six roots (shortAddLong, twoShortAddLong, threeShortAddLong, threeShortAddTwoLong with negatives), length relations via invariant forms (long = 3×short), complete pairing table for all root combinations, orthogonality lemma (roots outside 𝔤₂ span are orthogonal to basis), span_eq_top for irreducible systems, card_index_eq_twelve proving 𝔤₂ has exactly 12 roots |

## Subdirectories

(No subdirectories)

## Search Tags

finite-root-pairings canonical-bilinear-form polarization root-form invariant-forms weyl-invariance positive-definiteness coxeter-weights crystallographic classification nondegeneracy anisotropic root-lengths G2-root-system exceptional-lie-algebras root-closure root-chains pairing-enumeration dimensional-analysis
