---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/PFunctor/Univariate
generated: 2025-12-11T23:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 2
subdirs_count: 0
---

# Univariate

## Overview

This folder defines univariate polynomial functors and their fixed points. A polynomial functor `PFunctor` is a structure `(A : Type, B : A → Type)` that maps any type `α` to `Σ x : A, B x → α`. The folder provides both W-types (least fixed points, well-founded inductive trees) and M-types (greatest fixed points, potentially infinite coinductive trees). These constructions are foundational for defining quotients of polynomial functors (QPFs) used elsewhere in mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the `PFunctor` structure, its functor instance (`Obj`, `map`), proves it is a lawful functor, defines W-types as `WType P.B`, composition of polynomial functors (`comp`), and lifting of predicates/relations (`liftp`, `liftr`, `supp`) |
| M.lean | Defines M-types as the greatest fixed point/final coalgebra of a polynomial functor using approximation sequences (`CofixA`), provides corecursors (`corec`, `corec'`, `corec₁`), path-based traversal (`IsPath`, `isubtree`, `iselect`), and bisimulation-based equality proofs (`IsBisimulation`, `eq_of_bisim`) |

## Subdirectories

(none)

## Search Tags

pfunctor polynomial-functor univariate w-type m-type wtype mtype fixpoint cofixpoint corecursor bisimulation final-coalgebra approximation lawful-functor functor-composition predicate-lifting relation-lifting
