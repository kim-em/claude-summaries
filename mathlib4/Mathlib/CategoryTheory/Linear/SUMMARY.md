---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Linear
generated: 2025-12-07T10:25:26Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Linear

## Overview

The `Linear/` directory formalizes R-linear categories and functors, which are categories where morphism sets have R-module structure compatible with composition. An R-linear category requires hom-sets to be R-modules with composition being R-linear in both arguments (inheriting from preadditive categories). This framework provides the categorical foundation for linear algebra constructions, including linear functors that preserve the module structure on morphisms, functor category linearity, and a linear version of the Yoneda embedding valued in ModuleCat R.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of Linear R C typeclass requiring R-module structure on hom-sets with R-linear composition, includes canonical instances for ℕ and ℤ, algebra structure on endomorphism monoids, and linear composition maps (leftComp, rightComp) |
| LinearFunctor.lean | Linear functors between R-linear categories as additive functors preserving scalar multiplication on morphisms, with mapLinearMap bundling F.map as R-linear map and instances for identity, composition, and inverse functors |
| FunctorCategory.lean | R-linear structure on functor categories C ⥤ D when D is R-linear, with pointwise scalar multiplication on natural transformations and appLinearMap extracting component at fixed object |
| Yoneda.lean | Linear Yoneda embedding linearYoneda R C : C ⥤ Cᵒᵖ ⥤ ModuleCat R and coyoneda variant, sending objects to ModuleCat-valued (co)presheaves with proof of fully faithfulness |

## Subdirectories

*(No subdirectories)*

## Search Tags

linear-categories linear-functors enriched-categories module-categories yoneda-lemma preadditive-categories r-linear scalar-multiplication linear-maps functor-categories hom-modules categorical-algebra
