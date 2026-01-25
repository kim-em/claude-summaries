---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Defs
generated: 2026-01-26T10:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Defs

## Overview

The `Defs/` directory contains core definitional files for order theory, establishing the fundamental hierarchy from preorders through partial orders to linear orders. These files provide the essential typeclasses and unbundled relation classes (reflexivity, transitivity, antisymmetry, etc.) that underpin all order-theoretic reasoning in Mathlib. The directory includes definitions for covering relations (`⋖` and `⩿`), minimal/maximal elements, upper/lower sets, and basic lemmas establishing the properties of these fundamental order structures.

## Key Files

| File | Purpose |
|------|---------|
| Unbundled.lean | Unbundled relation classes (IsTrans, IsPreorder, IsPartialOrder, IsLinearOrder, IsStrictOrder, IsStrictWeakOrder, IsTrichotomous, IsEquiv) and their basic properties; defines Minimal/Maximal predicates and IsUpperSet/IsLowerSet/UpperSet/LowerSet types; provides fundamental lemmas for working with arbitrary binary relations |
| PartialOrder.lean | Preorder typeclass (reflexive + transitive) with strict order `<` defined as `a ≤ b ∧ ¬b ≤ a`; PartialOrder typeclass (preorder + antisymmetry); covering relations CovBy (`a ⋖ b`) and WCovBy (`a ⩿ b`); decidability instances for `<` and `=` from decidable `≤`; basic order lemmas (le_refl, le_trans, lt_irrefl, lt_trans, etc.) |
| LinearOrder.lean | LinearOrder typeclass (partial order + totality + decidable relations); min/max operations with their defining properties and commutativity/associativity lemmas; comparison function (compare) integration with Ord typeclass; proves totality-based lemmas (le_total, lt_or_ge, le_or_gt, lt_trichotomy) and comparison equivalences (compare_lt_iff_lt, compare_eq_iff_eq) |

## Subdirectories

*(none)*

## Search Tags

order-definitions preorder partial-order linear-order typeclass unbundled-relations reflexive transitive antisymmetric total trichotomous covering-relation wcovby covby minimal maximal upper-set lower-set decidable-order min-max compare ordering strict-order equivalence-relation
