---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Action/Pointwise/Set
generated: 2025-12-01T23:50:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Set

## Overview

The `Set/` directory implements pointwise group actions on sets, providing the core theory for how group actions lift from individual elements to entire sets. It defines typeclass instances showing that actions `M → α → α` naturally extend to `Set M → Set α → Set α` and `M → Set α → Set α`, along with comprehensive lemmas for how set operations (intersection, union, complement, difference) interact with scalar multiplication, translation properties under group actions, subset relationships involving action, and finiteness preservation under group actions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of pointwise actions on sets; defines `Set.mulAction` and `Set.mulActionSet` lifting monoid/group actions to sets, provides instances for `SMulCommClass`, `IsScalarTower`, `IsCentralScalar`, proves lemmas for set operations under actions (products, intersections, unions, complements, differences), establishes subset relationships and membership criteria involving `•`, includes translation/scaling properties and inversion distribution laws, proves coverage lemmas for translates of sets useful in approximate subgroup theory |
| Finite.lean | Finiteness preservation under pointwise actions; proves `finite_smul_set` and `infinite_smul_set` showing that scalar multiplication by a group element preserves finiteness/infiniteness of sets via bijectivity of group actions |

## Subdirectories

(none)

## Search Tags

pointwise set-action group-action scalar-multiplication smul set-operations translation scaling intersection union complement difference subset membership finiteness typeclass-instances smul-comm-class scalar-tower approximate-subgroup coverage inversion distribution mul-action
