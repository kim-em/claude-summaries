---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Monoid/Unbundled
generated: 2025-12-01T19:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 9
subdirs_count: 0
---

# Unbundled

## Overview

The `Unbundled/` directory provides the granular, unbundled foundation for ordered monoid theory by separating algebraic operations from order relations. Instead of bundled typeclasses like `OrderedMonoid`, it defines fine-grained properties through `CovariantClass` and `ContravariantClass`, which express precise monotonicity and reflection properties (e.g., "left multiplication preserves ≤", "right multiplication reflects <"). This unbundled approach enables flexible composition of assumptions, allowing lemmas to state exactly which properties they require without demanding full ordered monoid structures.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core unbundled framework: `CovariantClass` (action preserves relation), `ContravariantClass` (action reflects relation), with abbreviations `MulLeftMono`, `MulRightMono`, `MulLeftReflectLE`, etc. for common patterns |
| Basic.lean | Comprehensive ordered monoid lemmas using unbundled assumptions: monotonicity, cancellation, multiplication inequalities, comparison lemmas, and `MulLECancellable` predicate for order-reflecting elements |
| ExistsOfLE.lean | One-sided divisibility: `ExistsMulOfLE` (if `a ≤ b` then `∃ c, b = a * c`) and `ExistsAddOfLE`, weaker than canonical ordering but sufficient for many group-like arguments in monoid settings |
| MinMax.lean | Interaction of `min`/`max` with multiplication under monotonicity: distributivity lemmas (`min (a * b) (a * c) = a * min b c`), bounds (`max_le_mul_of_one_le`), and disjunctive comparison results |
| OrderDual.lean | Order dual instances: `MulLeftMono αᵒᵈ` from `MulLeftMono α` by flipping relations, automatically providing "dual" versions of all unbundled monotonicity properties |
| Pow.lean | Power/nsmul inequalities using unbundled covariance: monotonicity in base (`pow_le_pow_left'`) and exponent (`pow_le_pow_right'`), strict versions, and interaction with `1` (`one_le_pow_iff`) |
| TypeTags.lean | Unbundled order structures on `Multiplicative α` and `Additive α`: order instances transfer identically, `ExistsMulOfLE (Multiplicative α)` from `ExistsAddOfLE α`, equivalence lemmas for conversions |
| Units.lean | Units in ordered monoids: `Units.mulLECancellable_val` (unit values are LE-cancellable), inverse inequalities (`u⁻¹ * a ≤ b ↔ a ≤ u * b`), and `IsUnit` versions of cancellation lemmas |
| WithTop.lean | Adjoining `⊤` to ordered additive monoids: addition with top absorption (`⊤ + x = ⊤`), monotonicity instances (`AddLeftMono (WithTop α)`), cancellation for non-top elements, `ExistsAddOfLE` preservation, homomorphism extensions |

## Subdirectories

None.

## Search Tags

unbundled ordered-monoid covariant contravariant monotonicity reflection left-covariant right-covariant mul-le-cancellable exists-mul-of-le min-max power nsmul order-dual type-tags units with-top granular-typeclasses
