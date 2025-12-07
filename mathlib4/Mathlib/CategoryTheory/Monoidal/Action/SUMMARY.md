---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Action
generated: 2025-12-07T10:47:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 4
subdirs_count: 0
---

# Action

## Overview

The `Action/` directory formalizes the theory of actions of monoidal categories on arbitrary categories in mathlib4. It defines left and right actions of a monoidal category `C` on a category `D`, providing both structure classes and coherence axioms that mirror the monoidal category axioms. The directory includes the correspondence between actions and monoidal functors to endofunctor categories, linear functors that respect actions, and constructions relating actions to opposite and monoidal opposite categories. This framework generalizes the notion of group actions to categorical contexts and provides the foundation for module categories and representation theory in category theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of left and right actions with structure isomorphisms, coherence axioms, self-actions via tensor product, and bundled action functors `C ⥤ D ⥤ D` |
| End.lean | Equivalence between monoidal actions and monoidal functors to endofunctor categories with composition monoidal structure |
| LinearFunctor.lean | Lax, oplax, and strong linear functors compatible with left/right actions, with lineator morphisms and coherence conditions |
| Opposites.lean | Constructions relating actions on `C` and `D` to actions on opposite categories `Cᵒᵖ`, `Dᵒᵖ` and monoidal opposites `Cᴹᵒᵖ` |

## Subdirectories

(No subdirectories)

## Search Tags

monoidal-actions left-actions right-actions action-functors module-categories monoidal-functors endofunctor-categories linear-functors lineator opposite-actions monoidal-opposite category-actions representation-theory coherence-axioms bifunctors action-morphisms
