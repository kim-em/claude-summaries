---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Closed/FunctorCategory
generated: 2025-12-07T23:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 3
subdirs_count: 0
---

# FunctorCategory

## Overview

The `FunctorCategory/` directory provides constructions showing that functor categories inherit monoidal closed structure from their codomain. This includes both an explicit construction using enriched category theory (when the source is any category `J` and limits exist) and more abstract constructions for specific cases: functors from groupoids (using pointwise monoidal structure) and functors from arbitrary categories into complete monoidal closed categories (using adjoint lifting via comonadicity).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Explicit construction of monoidal closed structure on `J ⥤ C` when `C` is monoidal closed, using enriched homs and the functor enriched hom construction. Provides the bijection `(F₁ ⊗ F₂ ⟶ F₃) ≃ (F₂ ⟶ functorEnrichedHom C F₁ F₃)` and the adjunction `tensorLeft F ⊣ eHomFunctor` |
| Complete.lean | Abstract construction via comonadicity: shows functors `I ⥤ C` are monoidal closed when `C` is complete and monoidal closed, by lifting the adjunction from `Discrete I ⥤ C` using the comonadic left adjoint from the discrete inclusion |
| Groupoid.lean | Specialized construction for functors from groupoids: when `D` is a groupoid and `C` is monoidal closed, defines the internal hom `closedIhom F` as composition with the inverse functor, providing explicit unit/counit for the adjunction |

## Subdirectories

(No subdirectories)

## Search Tags

functor-category monoidal-closed internal-hom enriched-category enriched-hom adjunction groupoid comonadicity kan-extension discrete-category complete-category tensorLeft pointwise-monoidal curry uncurry evaluation coevaluation
