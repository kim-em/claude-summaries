---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Triangulated/Opposite
generated: 2025-12-08T07:11:57Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 4
subdirs_count: 0
---

# Opposite

## Overview

The `Opposite/` directory constructs the pretriangulated and triangulated structures on the opposite category Cᵒᵖ of a (pre)triangulated category C. The key innovation is defining the shift on Cᵒᵖ such that shifting by n on Cᵒᵖ corresponds to shifting by -n on C (not the standard opposite shift). This yields an anti-equivalence `triangleOpEquivalence : (Triangle C)ᵒᵖ ≌ Triangle Cᵒᵖ` that sends a distinguished triangle X → Y → Z → X⟦1⟧ in C to op Z → op Y → op X → (op Z)⟦1⟧ in Cᵒᵖ (without introducing signs). The directory proves that this construction makes Cᵒᵖ into a pretriangulated category where distinguished triangles are precisely those corresponding to distinguished triangles in C via the equivalence, and shows that a functor F : C → D is triangulated if and only if F.op is triangulated.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Constructs the custom shift on Cᵒᵖ via `OppositeShiftAux` and `PullbackShift`, where shifting by n on Cᵒᵖ equals shifting by -n on C; defines `shiftFunctorOpIso` and `opShiftFunctorEquivalence` auto-equivalence with detailed compatibility lemmas for unit/counit isomorphisms |
| Triangle.lean | Constructs the anti-equivalence `triangleOpEquivalence : (Triangle C)ᵒᵖ ≌ Triangle Cᵒᵖ` sending triangle X → Y → Z → X⟦1⟧ to op Z → op Y → op X → (op Z)⟦1⟧ without signs; defines functors in both directions with unit and counit isomorphisms |
| Pretriangulated.lean | Defines `distinguishedTriangles C` as triangles in Cᵒᵖ corresponding to distinguished triangles in C via triangleOpEquivalence; proves contractible triangles are distinguished, rotation preserves distinguished triangles, cocone completion, and morphism completion to establish pretriangulated structure on Cᵒᵖ |
| Functor.lean | Shows that a functor F : C → D commutes with shifts implies F.op commutes with shifts for the custom opposite shifts; proves compatibility of F.mapTriangle with triangleOpEquivalence via `mapTriangleOpCompTriangleOpEquivalenceFunctor`; establishes F.IsTriangulated iff F.op.IsTriangulated |

## Subdirectories

*(none)*

## Search Tags

opposite-category pretriangulated-structure triangulated-categories shift-functors distinguished-triangles opposite-shift triangle-equivalence verdier-duality functoriality triangulated-functors commuting-shifts anti-equivalence rotation-axiom completion-axiom homological-algebra
