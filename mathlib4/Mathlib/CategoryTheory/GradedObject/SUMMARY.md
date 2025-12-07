---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/GradedObject
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# GradedObject

## Overview

This directory contains advanced constructions for graded objects in category theory, extending the basic graded object framework from the parent `GradedObject.lean` file. The modules implement the monoidal category structure on graded objects (tensor products with coproducts indexed by addition), associator and unitor isomorphisms for bifunctor actions, braiding for commutative gradings, and support for bifunctors and trifunctors on graded objects. This infrastructure is essential for defining monoidal, braided, and symmetric category structures on graded objects indexed by additive monoids.

## Key Files

| File | Purpose |
|------|---------|
| Bifunctor.lean | Action of bifunctors `F : C₁ ⥤ C₂ ⥤ C₃` on graded objects, producing `GradedObject (I × J) C₃` and collapsing to `GradedObject K C₃` via maps `I × J → K` |
| Trifunctor.lean | Action of trifunctors on graded objects producing `GradedObject (I₁ × I₂ × I₃) C₄`, used for monoidal associator construction |
| Monoidal.lean | Monoidal category structure on `GradedObject I C` when `I` is an additive monoid and `C` is monoidal, tensor product via coproducts of `X₁ i ⊗ X₂ j` for `i + j = n` |
| Associator.lean | Associator isomorphism for bifunctor actions on graded objects, expressing `G(F₁₂(X₁, X₂), X₃) ≅ F(X₁, G₂₃(X₂, X₃))` |
| Unitor.lean | Left and right unitor isomorphisms for bifunctor actions on graded objects with unit objects from `single₀` functor |
| Braiding.lean | Braiding `tensorObj X Y ≅ tensorObj Y X` for graded objects over commutative additive monoids in braided categories, symmetry when `C` is symmetric |
| Single.lean | Functor `single j : C ⥤ GradedObject J C` placing an object in a single degree `j` with initial objects elsewhere |

## Subdirectories

*No subdirectories*

## Search Tags

graded-objects monoidal-categories tensor-products bifunctors trifunctors associator braiding symmetric-categories unitor additive-monoids coproducts homological-algebra
