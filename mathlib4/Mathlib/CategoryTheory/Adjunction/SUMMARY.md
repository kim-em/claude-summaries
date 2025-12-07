---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Adjunction
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 18
subdirs_count: 1
---

# Adjunction

## Overview

The `Adjunction/` directory contains the comprehensive formalization of adjoint functors in category theory, one of the most fundamental concepts connecting different categories. An adjunction `F ⊣ G` between functors `F : C ⥤ D` and `G : D ⥤ C` consists of a unit and counit natural transformation satisfying triangle identities. This directory provides multiple constructors for building adjunctions, characterizations of fully faithful adjoints, preservation theorems for limits and colimits, the adjoint functor theorems (both general and special), mate correspondence for 2-cells, reflective functors, adjoint lifting theorems, and various specialized constructions including whiskering, restrictions, triples, and uniqueness results.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core adjunction structure with unit/counit, `F ⊣ G` notation, various constructors (`mkOfHomEquiv`, `mk'`, `leftAdjointOfEquiv`), composition of adjunctions, conversion to/from equivalences, and typeclasses `IsLeftAdjoint`/`IsRightAdjoint` |
| FullyFaithful.lean | Characterization of fully faithful adjoints: left adjoint is faithful/full/fully-faithful iff unit is mono/split-epi/iso, right adjoint is faithful/full/fully-faithful iff counit is epi/split-mono/iso (Riehl 4.5.13) |
| Limits.lean | Preservation theorems: left adjoints preserve colimits, right adjoints preserve limits, equivalences create and reflect (co)limits, natural isomorphism between cocones over `K ⋙ F` and cocones over `K` with cone point `G.obj Y` |
| AdjointFunctorTheorems.lean | General adjoint functor theorem (functor preserving limits with solution set condition has left adjoint) and special adjoint functor theorem (for complete well-powered categories with small coseparating set), plus corollaries about completeness implying cocompleteness |
| Mates.lean | Mate correspondence establishing bijection between 2-cells in adjoint squares, showing adjoints are unique up to isomorphism, and applications to exponential comparison morphisms and Frobenius reciprocity |
| Reflective.lean | Reflective functors (fully faithful right adjoints) with reflector construction and essential properties |
| Comma.lean | Equivalence between left adjoint to `G` and initial objects in each `StructuredArrow` category on `G` (plus dual for right adjoints) |
| Evaluation.lean | Adjunctions between evaluation functors and product/coproduct constructions |
| Triple.lean | Adjoint triples `F ⊣ G ⊣ H` with theorem that `F` is fully faithful iff `H` is, and canonical natural transformations `H ⟶ F` (when `G` fully faithful) and `F ⟶ H` (when `F` and `H` fully faithful) |
| Unique.lean | Uniqueness of adjoints up to natural isomorphism |
| Whiskering.lean | Whiskering adjunctions with functors to induce adjunctions between functor categories: `F ⊣ G` induces adjunctions `C ⥤ D` and `C ⥤ E`, and between `E ⥤ C` and `D ⥤ C` |
| Opposites.lean | Constructions relating adjunctions of functors to adjunctions of their opposite functors |
| Restrict.lean | Restriction of adjunctions along fully faithful functors |
| PartialAdjoint.lean | Partial adjoints defined on subcategories or satisfying weaker conditions |
| Parametrized.lean | Parametrized adjunctions depending on additional data |
| Quadruple.lean | Adjoint quadruples and their properties |
| CompositionIso.lean | Isomorphisms arising from composition of adjunctions |
| Additive.lean | Adjunctions in additive categories preserving additive structure |

## Subdirectories

- [ ] `Lifting/` - Adjoint triangle theorem and adjoint lifting theorem for constructing left adjoints from monadic functors and commutative squares (pending)

## Search Tags

adjunction adjoint-functors unit counit left-adjoint right-adjoint fully-faithful reflective-functors adjoint-functor-theorem mate-correspondence limit-preservation colimit-preservation adjoint-lifting monadic-functors equivalence natural-isomorphism whiskering solution-set-condition
