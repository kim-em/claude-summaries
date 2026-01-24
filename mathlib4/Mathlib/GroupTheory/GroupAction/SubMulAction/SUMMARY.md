---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/GroupAction/SubMulAction
generated: 2026-01-24T11:24:22Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# SubMulAction

## Overview

The `SubMulAction/` directory contains specialized theory for sub-mul-actions in group action contexts. It provides constructions for creating SubMulActions from stabilizers and fixing subgroups, closure operations for generating SubMulActions from sets, combinations (finite subsets of fixed cardinality with group actions), and pointwise monoid structures on SubMulActions. Key applications include studying multiple transitivity through stabilizer actions on complements, and manipulating SubMulActions via equivariant maps between various related structures.

## Key Files

| File | Purpose |
|------|---------|
| OfStabilizer.lean | SubMulAction of the stabilizer of a point on the complement: `ofStabilizer G a` for `stabilizer G a` acting on `{a}ᶜ`, with equivariant maps between translates and embedding constructions |
| OfFixingSubgroup.lean | SubMulAction of fixing subgroup on complement of invariant subset: `ofFixingSubgroup M s` for `fixingSubgroup M s` acting on `sᶜ`, with extensive equivariant map machinery for relating different fixing subgroup actions |
| Closure.lean | Closure and finiteness of SubMulAction/SubAddAction: `closure R s` generates the smallest SubMulAction containing set `s`, with finitely generated (FG) predicate |
| Combination.lean | Combinations (finite subsets of fixed cardinality) with group actions: `Nat.Combination α n` for n-element subsets, with SubMulAction structure, equivariant maps from embeddings, pretransitivity results, and complement operations |
| Pointwise.lean | Pointwise monoid structures on SubMulAction: Mul, One, MulOneClass, Semigroup, Monoid instances for SubMulActions that inherit pointwise operations from sets |

## Subdirectories

## Search Tags

sub-mul-action stabilizer fixing-subgroup closure finitely-generated combination pointwise equivariant-map multiple-transitivity complement faithful-action pretransitive
