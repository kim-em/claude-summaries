---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/PFunctor/Multivariate
generated: 2025-12-11T21:45:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 3
subdirs_count: 0
---

# Multivariate

## Overview

This directory defines multivariate polynomial functors (`MvPFunctor`) and their fixed points: M-types (greatest fixpoints, potentially infinite trees) and W-types (least fixpoints, well-founded trees). Multivariate polynomial functors map type vectors `TypeVec n` to types via the construction `Sigma a : A, B a ==> alpha`, where `A` is the "head" type and `B : A -> TypeVec n` is the "child family". These are fundamental for defining quotients of polynomial functors (QPFs) used to construct inductive and coinductive datatypes in Lean.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `MvPFunctor` structure with head type `A` and child family `B`, proves it forms a lawful functor, provides constant functors (`const`) and functor composition (`comp`), and includes lifting lemmas for predicates/relations |
| M.lean | Defines M-types as greatest fixpoints via `M.Path` (potentially infinite paths), provides corecursor `M.corec` for coinductive definitions, destructor `M.dest`, and bisimulation principle `M.bisim` for proving equality of coinductive values |
| W.lean | Defines W-types as least fixpoints via `WPath` (well-founded paths), provides constructor `wMk`, recursor `wRec` for structural recursion, induction principle `w_ind`, and destructor `wDest'` for pattern matching |

## Subdirectories

(none)

## Search Tags

multivariate-polynomial-functors mvpfunctor m-types w-types coinductive inductive greatest-fixpoint least-fixpoint corecursor bisimulation well-founded-trees infinite-trees typevec functor-composition qpf
