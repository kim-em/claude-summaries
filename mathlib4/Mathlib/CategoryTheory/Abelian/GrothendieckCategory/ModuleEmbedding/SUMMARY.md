---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Abelian/GrothendieckCategory/ModuleEmbedding
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# ModuleEmbedding

## Overview

The `ModuleEmbedding/` directory proves fundamental embedding theorems for Grothendieck abelian categories into module categories. The Gabriel-Popescu theorem establishes that every Grothendieck abelian category with separator G embeds fully faithfully into ModuleCat (End G)ᵐᵒᵖ via the coyoneda functor Hom(G, ·), with an exact left adjoint (tensor product). The opposite embedding theorem constructs embeddings of Cᵒᵖ into module categories that are faithful, exact, and preserve finite limits and colimits.

## Key Files

| File | Purpose |
|------|---------|
| GabrielPopescu.lean | Proves the Gabriel-Popescu theorem following Barry Mitchell's elementary proof; constructs the tensor-hom adjunction (· ⊗ G) ⊣ Hom(G, ·), proves that preadditiveCoyonedaObj G is fully faithful and its left adjoint tensorObj G preserves finite limits; establishes fullness using separator property and injectiveness preservation via Baer's criterion |
| Opposite.lean | Constructs embeddings of opposite categories Cᵒᵖ into module categories for functors F : D ⥤ Cᵒᵖ from small categories; builds a projective separator from the coseparator, constructs a generator as coproduct over F's image, proves the embedding functor is faithful, exact, and preserves finite (co)limits; shows F ⋙ embedding F is full when F is full |

## Subdirectories

None.

## Search Tags

gabriel-popescu module-embedding grothendieck-categories coyoneda tensor-hom-adjunction fully-faithful-functor exact-functor separator baer-criterion projective-separator opposite-category embedding-ring preserves-limits mitchell-theorem
