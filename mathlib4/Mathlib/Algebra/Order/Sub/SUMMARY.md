---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Sub
generated: 2025-12-01T12:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 4
subdirs_count: 1
---

# Sub

## Overview

The `Sub/` directory provides a comprehensive theory of ordered subtraction, introducing the `OrderedSub` typeclass which characterizes subtraction via the property `a - b ≤ c ↔ a ≤ c + b`. This framework elegantly unifies both normal subtraction in ordered groups and truncated subtraction (tsub) in canonically ordered monoids like `ℕ`, `Multiset`, and `ENNReal`. The directory spans from core definitions (Defs.lean) through bundled theory (Basic.lean) to specialized constructions (Prod.lean, WithTop.lean), with a dedicated `Unbundled/` subdirectory providing the full theory for structures with `ExistsAddOfLE` before they're bundled into canonically ordered monoids. The unbundled approach enables fine-grained control via `AddLECancellable` and proves that additive homomorphisms weakly preserve tsub with exact preservation under suitable conditions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `OrderedSub` typeclass defining the fundamental characterization `a - b ≤ c ↔ a ≤ c + b`, with lemmas for preorders, partial orders, and linear orders including monotonicity (`tsub_le_tsub`), commutativity (`tsub_right_comm`), and strict inequalities (`lt_tsub_iff_right`) |
| Basic.lean | Lemmas for bundled canonically ordered monoids with `OrderedSub`: key results include `tsub_eq_zero_iff_le`, `tsub_self`, `tsub_pos_iff_lt`, `tsub_lt_self_iff`, cancellation lemmas (`add_tsub_cancel_of_le`), and specialized results for linear orders including `tsub_tsub_eq_min` and `tsub_add_eq_max` |
| Prod.lean | `OrderedSub` instances for product types (`α × β`) and Pi types (`(i : ι) → α i`), proving componentwise ordered subtraction |
| WithTop.lean | Subtraction on `WithTop α` for types with bottom element (targeting `ℕ∞`, `ℝ≥0∞`): defines `x - ⊤ = ⊥` and `⊤ - x = ⊤`, with simp lemmas and `OrderedSub` instance |

## Subdirectories

- [x] `Unbundled/` - Extended theory for unbundled canonically ordered monoids and homomorphism preservation

## Search Tags

ordered-subtraction truncated-subtraction tsub ordered-sub canonically-ordered-monoid additive-monoid ordered-group subtraction-characterization monotonicity cancellation homomorphism-preservation product-types pi-types with-top ennreal nat-subtraction multiset unbundled-structures exists-add-of-le add-le-cancellable
