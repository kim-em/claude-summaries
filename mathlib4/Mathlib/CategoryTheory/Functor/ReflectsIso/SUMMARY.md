---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Functor/ReflectsIso
generated: 2025-12-07T19:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# ReflectsIso

## Overview

The `ReflectsIso/` directory defines functors that reflect isomorphisms - functors `F : C ⥤ D` where if `F.map f` is an isomorphism, then `f` was already an isomorphism in the source category. This is formalized as the `Prop`-valued typeclass `ReflectsIsomorphisms F`. The module establishes that fully faithful functors reflect isomorphisms, that reflection of isomorphisms is closed under composition, and relates reflection of isomorphisms to balanced categories via reflection/preservation of monomorphisms and epimorphisms.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `ReflectsIsomorphisms` typeclass: `F.map f` is iso implies `f` is iso; instances showing fully faithful functors reflect isos, composition preserves reflection, and whiskering right preserves reflection |
| Balanced.lean | Connection to balanced categories: in balanced categories, reflecting epis and monos implies reflecting isos; conversely, reflecting isos + preserving epis/monos allows transferring balanced property |

## Subdirectories

*(none - leaf folder)*

## Search Tags

functors reflects-isomorphisms category-theory fully-faithful balanced-categories epimorphisms monomorphisms isomorphisms typeclass composition whiskering
