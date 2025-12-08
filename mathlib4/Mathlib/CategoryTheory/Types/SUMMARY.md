---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Types
generated: 2025-12-08T15:42:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# Types

## Overview

This directory contains the formalization of Lean's type universe as a large category, establishing `Type u` as a categorical object where morphisms are functions. It proves fundamental correspondences between categorical and type-theoretic concepts: monomorphisms are injections, epimorphisms are surjections, and categorical isomorphisms correspond exactly to type equivalences. The directory also provides infrastructure for functors valued in types (sections, naturality lemmas, universe lifting) and establishes stability properties of monomorphisms under categorical constructions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core category instance for `Type u` with morphisms as functions, simplification lemmas for functors/natural transformations to types, sections functor, `uliftFunctor` for universe lifting (fully faithful), correspondence between `Iso` and `Equiv`, characterization of monos (injections), epis (surjections), and isos (bijections), conversion from lawful type functors to categorical functors |
| Monomorphisms.lean | Stability properties of monomorphisms in `Type u`: stable under cobase change (pushouts), stable under filtered colimits, with automatic transfinite composition stability when appropriate imports are present |
| Set.lean | Functor `Set.functorToTypes : Set X ⥤ Type u` sending each set `A : Set X` to its underlying type with morphisms given by set inclusions |

## Subdirectories

*(No subdirectories)*

## Search Tags

type-category types-as-category function-category categorical-types monomorphisms-injections epimorphisms-surjections iso-equiv-correspondence sections-functor ulift-functor universe-lifting type-functor stability-properties filtered-colimits cobase-change set-functor
