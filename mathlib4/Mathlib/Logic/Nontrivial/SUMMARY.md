---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Logic/Nontrivial
generated: 2026-01-25T19:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Nontrivial

## Overview

The `Nontrivial/` subdirectory formalizes the property of types containing at least two distinct elements. The `Nontrivial` typeclass is fundamental in algebra (distinguishing rings where 0 ≠ 1) and linear algebra (ensuring positive dimension in vector spaces). The directory splits cleanly into definitions (`Defs.lean`) establishing the typeclass and basic constructors, and additional results (`Basic.lean`) covering linear orders, subtypes, product types, pi types, and the relationship with `Unique` types.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `Nontrivial` typeclass definition requiring `∃ x y : α, x ≠ y`; includes basic lemmas (nontrivial_iff, exists_ne, nontrivial_of_ne), propagation through injective/surjective functions, relationship with `Subsingleton` (complementary via `not_nontrivial_iff_subsingleton`), and instances for `Prop` and `Bool` |
| Basic.lean | Extended nontrivial results requiring more imports; includes order-based constructors (`nontrivial_of_lt`, `exists_pair_lt` for linear orders), `nontrivialPSumUnique` dichotomy for inhabited types, `Subtype.nontrivial_iff_exists_ne`, and instances for `Option`, products, pi types, and function spaces; depends on Data.Prod, Logic.Function, Logic.Unique, and Order.Defs |

## Subdirectories

*(none)*

## Search Tags

nontrivial typeclass two-elements distinct-elements rings vector-spaces subsingleton unique linear-order product-types pi-types function-spaces mathlib logic
