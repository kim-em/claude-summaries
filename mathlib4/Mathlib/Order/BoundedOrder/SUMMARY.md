---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/BoundedOrder
generated: 2026-01-25T22:30:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 3
subdirs_count: 0
---

# BoundedOrder

## Overview

The `BoundedOrder/` subdirectory contains the foundational theory of bounded orders—orders equipped with top (`⊤`) and bottom (`⊥`) elements. Basic.lean defines the core typeclasses (OrderTop, OrderBot, BoundedOrder) and establishes fundamental lemmas for working with greatest and least elements across partial orders, linear orders, and product/subtype constructions. Lattice.lean adds bounded lattice operations (supremum/infimum with top/bottom), while Monotone.lean provides specialized results about monotone and antitone functions on bounded orders, including characterizations of strictness and logical monotonicity on Prop.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core typeclasses for orders with top/bottom elements: OrderTop (with le_top), OrderBot (with bot_le), BoundedOrder; fundamental theorems (top_unique, eq_top_iff, lt_top_iff_ne_top, subsingleton_of_bot_eq_top); instances for OrderDual, Pi types, products, subtypes, ULift, and Bool |
| Lattice.lean | Bounded lattice lemmas: interaction of ⊔/⊓ with ⊤/⊥ (top_sup_eq, bot_inf_eq, sup_eq_bot_iff, inf_eq_top_iff); min/max operations with top/bottom in linear orders; WellFoundedGT.induction_top for well-founded induction to top element |
| Monotone.lean | Monotonicity on bounded orders: StrictMono.apply_eq_top_iff and apply_eq_bot_iff characterizations; maximal/minimal preimage results; monotonicity of logical operations on Prop (monotone_and, monotone_or, monotone_le, Monotone.forall, Monotone.exists, forall_ge_iff) |

## Subdirectories

## Search Tags

bounded-order top bottom OrderTop OrderBot BoundedOrder greatest-element least-element le_top bot_le bounded-lattice supremum infimum monotone antitone strict-mono logical-monotonicity Prop
