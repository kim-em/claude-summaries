---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Comma/Over
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 3
subdirs_count: 0
---

# Over

## Overview

The `Over/` directory implements over categories (slice categories) and under categories (coslice categories), which are special cases of comma categories. An over category `Over X` has objects consisting of morphisms with codomain `X` and morphisms given by commutative triangles. Dually, an under category `Under X` has objects consisting of morphisms with domain `X`. The directory includes the basic definitions, typeclass-based interfaces for working with structure morphisms, and pullback/pushout functors that relate over/under categories via adjunctions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of over and under categories with objects as morphisms to/from a fixed object, morphism constructors (`homMk`, `isoMk`), forgetful functors, map functors induced by morphisms, equivalences (iterated slice, post functors), and structured/costructured arrow conversions |
| OverClass.lean | Typeclass infrastructure for working with structure morphisms: `OverClass X S` provides `X ↘ S : X ⟶ S`, `HomIsOver f S` asserts commutativity with structure morphisms, bundling/unbundling between typeclasses and `Over/Under` categories |
| Pullback.lean | Adjunctions relating over/under categories: pullback functor `Over Y ⥤ Over X` induced by `f : X ⟶ Y` (right adjoint to `map f`), pushout functor `Under X ⥤ Under Y` (left adjoint to `map f`), star/costar functors relating categories to their over/under categories via binary products/coproducts |

## Subdirectories

*(No subdirectories)*

## Search Tags

over-category under-category slice-category coslice-category structure-morphism pullback-functor pushout-functor adjunction typeclass-interface star-functor costar-functor iterated-slice
