---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Monoid
generated: 2025-12-01T20:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 14
subdirs_count: 2
---

# Monoid

## Overview

The `Monoid/` directory provides comprehensive ordered monoid theory through both bundled and unbundled approaches. At the bundled level, it defines core typeclasses (`IsOrderedMonoid`, `IsOrderedCancelMonoid`) for monotone multiplication and cancellation, with specialized variants like `CanonicallyOrderedMul` where ordering exactly corresponds to divisibility. At the unbundled level, it provides fine-grained building blocks (`CovariantClass`, `ContravariantClass`) that enable precise statement of monotonicity assumptions without requiring full ordered monoid structures. The directory establishes ordered instances on standard constructions (products, order duals, submonoids, units, type tags, WithTop/WithBot), proves foundational properties including unique units in canonical orderings, and develops specialized theory for locally finite orders, associates, and natural number numerals.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclasses: `IsOrderedMonoid` (multiplication monotone), `IsOrderedCancelMonoid` (cancellative monotone multiplication), with instances and self-multiplication lemmas |
| Basic.lean | Additional ordered monoid theory: pullback constructions under injective/strict monotone maps, order embeddings `mulLeft`/`mulRight` |
| Associated.lean | Associates in cancel commutative monoids with zero form canonically ordered monoids under divisibility ordering |
| Lex.lean | Order homomorphisms for products: natural inclusions/projections for both plain products (`α × β`) and lexicographic products (`α ×ₗ β`) |
| LocallyFiniteOrder.lean | Locally finite linearly ordered abelian groups are isomorphic to `ℤ` (additive) or `Multiplicative ℤ` (multiplicative) or `ℤᵐ⁰` (with zero) |
| NatCast.lean | Order of numerals in ordered additive monoids: `0 ≤ 1 < 2 < 3 < 4`, with `NeZero` instances and lemmas like `lt_add_one` |
| OrderDual.lean | Ordered monoid structures on order dual: `IsOrderedMonoid αᵒᵈ` and `IsOrderedCancelMonoid αᵒᵈ` instances |
| PNat.lean | Equivalence `ℕ+ ≃*o nonZeroDivisors ℕ` between positive naturals and non-zero divisors of ℕ |
| Prod.lean | Product instances: `IsOrderedMonoid (α × β)`, `IsOrderedCancelMonoid (α × β)`, `CanonicallyOrderedMul (α × β)`, plus lexicographic variants |
| Submonoid.lean | Submonoids of ordered monoids inherit ordered structure; defines `oneLE` submonoid of elements `≥ 1` |
| ToMulBot.lean | Equivalence between `WithZero (Multiplicative α)` and `Multiplicative (WithBot α)` for additive monoids |
| TypeTags.lean | Ordered monoid instances for `Multiplicative α` and `Additive α` type tags, transferring between additive and multiplicative structures |
| Units.lean | Units of ordered monoids inherit order structure, with `val` as order embedding; defines max/min/linear order instances |
| WithTop.lean | Adjoining top/bottom elements: `IsOrderedAddMonoid (WithTop α)` and `CanonicallyOrderedAdd` instances for `WithTop`/`WithBot` |

## Subdirectories

- [x] `Canonical/` - Canonically ordered monoids where `a ≤ b ↔ ∃c, b = a * c` exactly, with unique units theorem and `Finset.sup` properties
- [x] `Unbundled/` - Fine-grained monotonicity framework using `CovariantClass`/`ContravariantClass`, with power/min/max lemmas, `ExistsMulOfLE` weaker divisibility, and cancellation predicates

## Search Tags

ordered-monoid ordered-cancel-monoid monotone-multiplication cancellation product-monoid lexicographic-product order-dual submonoid units associates locally-finite natural-numbers numerals type-tags multiplicative-additive with-top with-bot canonical-order canonically-ordered-monoid divisibility-order exists-mul-of-le exists-add-of-le unique-units unbundled covariant-class contravariant-class left-covariant right-covariant mul-le-cancellable reflection granular-typeclasses power nsmul min-max
