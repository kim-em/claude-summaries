---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/EffectiveEpi
generated: 2025-12-07T09:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# EffectiveEpi

## Overview

The `EffectiveEpi/` directory formalizes effective epimorphisms and effective epimorphic families in category theory. An effective epimorphism is a morphism that exhibits its codomain as a colimit of all pairs of morphisms it coequalizes (often called "strict epi" in the literature). The directory provides the core definitions, proves composition and decomposition properties, establishes relationships with coproducts and descent theory, and develops the theory of functors that preserve or reflect these structures. This machinery is essential for descent theory, site theory, and the study of Grothendieck topologies.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `EffectiveEpi` and `EffectiveEpiFamily` with descent operations, universal properties, and basic instances (isomorphisms, coproducts inducing isos) |
| Comp.lean | Composition properties: effective epis precomposed with split epis remain effective, effective epi families postcomposed with isos remain effective |
| Coproduct.lean | Bidirectional relationship between effective epi families and effective epis from coproducts (when pullbacks interact well with coproducts) |
| Enough.lean | `EffectivelyEnough` property for functors: every object in the target category admits an effective epi from an object in the functor's image |
| Extensive.lean | Specialization to finitary pre-extensive categories: effective epi families correspond to effective epis from coproducts via `Sigma.desc` |
| Preserves.lean | Functors preserving/reflecting effective epis and families, including classes `PreservesEffectiveEpis`, `ReflectsEffectiveEpis`, with equivalences as instances |
| RegularEpi.lean | Deprecated module (since 2025-11-20) redirecting to `Mathlib.CategoryTheory.Limits.Shapes.RegularMono` |

## Subdirectories

(None)

## Search Tags

effective-epimorphism effective-epi descent coequalizer strict-epi effective-epi-family universal-property composition coproduct extensive-category preserve-reflect functorial-property site-theory descent-theory
