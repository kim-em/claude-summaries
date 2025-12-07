---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Functor/KanExtension
generated: 2025-12-07T19:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 6
subdirs_count: 0
---

# KanExtension

## Overview

The `KanExtension/` directory provides a comprehensive formalization of Kan extensions in category theory. It defines left and right Kan extensions of functors as universal objects in categories of extensions, introduces pointwise Kan extensions characterized by (co)limits, establishes Kan extension functors and their adjunctions with precomposition functors, and includes specialized results for dense functors and preservation of Kan extensions under various conditions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of left/right Kan extensions via `IsLeftKanExtension` and `IsRightKanExtension` typeclasses, universal properties, lifting operations, and uniqueness results |
| Pointwise.lean | Pointwise Kan extensions defined via (co)limits: `HasPointwiseLeftKanExtensionAt` using colimits of `CostructuredArrow.proj L Y ⋙ F` and dual for right extensions |
| Adjunction.lean | Kan extension functors `L.lan : (C ⥤ H) ⥤ (D ⥤ H)` and `L.ran : (C ⥤ H) ⥤ (D ⥤ H)` with adjunction to precomposition functors, plus isomorphisms to (co)limits |
| Dense.lean | Dense functors (`F.IsDense`) where the identity functor is a pointwise left Kan extension of `F` along itself, with equivalence to fully faithful restricted Yoneda embedding |
| DenseAt.lean | Pointwise density condition `F.DenseAt Y` expressing that `Y` is a canonical colimit of `F.obj X` over all `F.obj X ⟶ Y`, with stability under isomorphisms and equivalences |
| Preserves.lean | Preservation of Kan extensions by functors via `PreservesLeftKanExtension` and `PreservesRightKanExtension` typeclasses, with constructors for pointwise cases |

## Subdirectories

(none)

## Search Tags

kan-extensions left-kan-extension right-kan-extension pointwise-kan-extension adjunction category-theory dense-functors universal-property preservation colimits limits structured-arrows costructured-arrows
