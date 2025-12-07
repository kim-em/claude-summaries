---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/PathCategory
generated: 2025-12-07T11:26:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# PathCategory

## Overview

The `PathCategory/` directory formalizes the path category construction for quivers, which turns any quiver (directed graph) into a category where objects are vertices and morphisms are paths between vertices. The construction provides a universal property: any prefunctor from a quiver lifts uniquely to a functor from its path category. For categories viewed as quivers, there is an equivalence showing that the quotient of the path category by the relation "paths compose to the same morphism" recovers the original category.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core path category construction `Paths V` with category instance, lifting prefunctors to functors via universal property, induction principles for reasoning about morphisms, composition of paths in categories via `composePath` and `pathComposition` functor, and equivalence between quotient of path category and original category |
| MorphismProperty.lean | Reformulation of path category induction principles in terms of `MorphismProperty`, proving properties equal to top (always true) given base cases and composition closure, and construction of natural transformations/isomorphisms between functors out of path categories from componentwise data |

## Subdirectories

*(none)*

## Search Tags

path-category quiver free-category universal-property prefunctor-lifting induction-principles quotient-equivalence morphism-property natural-transformation
