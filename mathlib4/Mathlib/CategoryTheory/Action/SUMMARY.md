---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Action
generated: 2025-12-07T07:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 5
subdirs_count: 0
---

# Action

## Overview

The `Action/` directory formalizes the categorical treatment of monoid and group actions within an arbitrary category `V`. The core construction `Action V G` bundles an object of `V` with a monoid homomorphism `G →* End V`, capturing how elements of a monoid `G` act on that object. When `V = ModuleCat R`, this yields linear representations of `G`; when `V = Type`, it gives ordinary `G`-sets. The directory establishes the equivalence `Action V G ≌ (singleObj G ⥤ V)` and shows that categorical properties (limits, colimits, monoidal structure, preadditive/abelian structure) lift from `V` to `Action V G`. Additional structure includes continuous actions on topological categories and monoidal category structure on actions when the underlying category is monoidal.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `Action V G` structure with morphisms, category instance, equivalence to functor category `singleObj G ⥤ V`, and restriction functors along monoid homomorphisms |
| Concrete.lean | Constructors for actions in concrete categories, particularly `Action (Type*) G` from `MulAction` instances, product constructions, orbit and stabilizer subgroups, and quotient actions |
| Continuous.lean | Continuous actions on topological categories via `ContAction V G` and `DiscreteContAction V G` as full subcategories where induced actions are continuous |
| Limits.lean | Categorical properties showing `Action V G` inherits limits, colimits, preadditive structure, linear structure, and abelian structure from `V` via the functor category equivalence |
| Monoidal.lean | Monoidal category structure on `Action V G` when `V` is monoidal, including braided and symmetric structures, transported via functor category equivalence |

## Subdirectories

(No subdirectories)

## Search Tags

action representation group-action monoid-action functor-category concrete-category monoidal-category limits colimits abelian preadditive continuous-action topological-action restriction-functor orbit stabilizer quotient-action
