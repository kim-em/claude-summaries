---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Preadditive/Projective
generated: 2025-12-07T13:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 5
subdirs_count: 0
---

# Projective

## Overview

The `Projective/` directory contains the formalization of projective objects in preadditive categories. A projective object `P` is one where every morphism out of `P` factors through any epimorphism. This includes the core definition and characterizations of projective objects, projective presentations, categories with enough projectives, internal projectivity in monoidal closed categories, characterizations via lifting properties, preservation of projective objects by functors, and projective resolutions as chain complexes of projective objects used in homological algebra.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of projective objects and categories with enough projectives; includes `Projective P` typeclass (morphisms out of P factor through epis), `ProjectivePresentation X` structure (epi from projective to X), `EnoughProjectives C` class, factorization constructions, preservation under isomorphisms and coproducts/biproducts, characterization via coyoneda preserving epis, and adjunction/equivalence results |
| Internal.lean | Internal projectivity in monoidal closed categories: `InternallyProjective P` means the internal hom functor `P ⟶[C] -` preserves epimorphisms; proves stability under retracts |
| LiftingProperties.lean | Characterizes projective objects via lifting properties: proves `P` is projective iff `0 ⟶ P` has the left lifting property with respect to all epimorphisms |
| Preserves.lean | Functor preservation of projective objects: defines `Functor.PreservesProjectiveObjects` typeclass, proves left adjoints preserve projective objects when right adjoint preserves epis, and conversely shows right adjoints preserve epis when left adjoint preserves projectives (requires enough projectives) |
| Resolution.lean | Projective resolutions for homological algebra: `ProjectiveResolution Z` is an ℕ-indexed chain complex of projective objects with quasi-isomorphism to the single complex with Z in degree 0; includes exactness properties, cokernel characterizations, and functorial mapping of resolutions |

## Subdirectories

None.

## Search Tags

projective-objects projective-presentations enough-projectives factorization epimorphisms lifting-properties internal-projectivity monoidal-closed coyoneda preserving-epimorphisms adjunctions equivalences coproducts biproducts projective-resolutions chain-complexes quasi-isomorphisms homological-algebra
