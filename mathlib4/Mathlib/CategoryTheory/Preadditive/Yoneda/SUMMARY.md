---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Preadditive/Yoneda
generated: 2025-12-07T11:36:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Yoneda

## Overview

The `Yoneda/` directory contains the specialization of the Yoneda embedding for preadditive categories. In the preadditive setting, the Yoneda functor sends an object Y to a presheaf valued in AddCommGrpCat (the category of abelian groups), with each hom-set carrying an additional End Y-module structure. This directory establishes that the preadditive Yoneda embedding is fully faithful, additive, preserves limits, and characterizes injective and projective objects via epimorphism preservation properties.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of preadditive Yoneda and coyoneda embeddings that lift to AddCommGrpCat and ModuleCat; proves these are fully faithful and additive, compatible with the ordinary Yoneda embedding via forgetful functors |
| Limits.lean | Shows that preadditiveYonedaObj and preadditiveCoyonedaObj preserve all limits; uses the abelian structure on ModuleCat to lift limit preservation from the underlying Yoneda embedding |
| Injective.lean | Characterizes injective objects in preadditive categories: an object J is injective iff preadditiveYoneda.obj J (or preadditiveYonedaObj J) preserves epimorphisms |
| Projective.lean | Characterizes projective objects in preadditive categories: an object P is projective iff preadditiveCoyoneda.obj P (or preadditiveCoyonedaObj P) preserves epimorphisms |

## Subdirectories

*(No subdirectories)*

## Search Tags

yoneda-embedding preadditive-yoneda coyoneda additive-functors module-structure endomorphism-ring fully-faithful preserves-limits injective-characterization projective-characterization epimorphism-preservation presheaves copresheaves
