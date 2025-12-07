---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Comma/Presheaf
generated: 2025-12-07T08:50:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Presheaf

## Overview

The `Presheaf/` directory establishes fundamental connections between comma categories and presheaf categories, specifically relating the over category `Over A` for a presheaf `A : Cᵒᵖ ⥤ Type v` to the category of presheaves on costructured arrows. The main result is a categorical equivalence showing that `Over A ≌ (CostructuredArrow yoneda A)ᵒᵖ ⥤ Type v`, which in Kashiwara-Schapira notation is written as `C^ₐ ≌ Cₐ^`. This equivalence fits into a quasi-commutative diagram involving the Yoneda embedding and forgetful functors, and is used to prove relative versions of the Yoneda lemma's preservation of colimits.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Constructs the equivalence `overEquivPresheafCostructuredArrow` between `Over A` and presheaves on `(CostructuredArrow yoneda A)ᵒᵖ`, proving the quasi-commutative triangle with the Yoneda embedding and forgetful functor; includes detailed technical machinery for handling dependent type theory correction terms |
| Colimit.lean | Proves relative Yoneda preserves certain colimits: for functors `F : J ⥤ Over A`, establishes natural isomorphism `Hom(YX, colim_i Fi) ≅ colim_i Hom(YX, Fi)` where `Y` is the relative Yoneda embedding `CostructuredArrow.toOver yoneda A` |

## Subdirectories

None.

## Search Tags

presheaf over-category yoneda-lemma costructured-arrow categorical-equivalence colimit-preservation kashiwara-schapira relative-yoneda comma-category
