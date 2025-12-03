---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Sub/Unbundled
generated: 2025-12-01T12:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Unbundled

## Overview

The `Unbundled/` directory provides the full theory of ordered subtraction for unbundled canonically ordered monoids—those with `ExistsAddOfLE` rather than the bundled `CanonicallyOrderedAddCommMonoid`. Basic.lean establishes fundamental cancellation, associativity, and comparison results, with fine-grained control via `AddLECancellable` for structures where not all elements cancel. Hom.lean proves that additive homomorphisms weakly preserve tsub, with exact preservation under suitable conditions, and that order isomorphisms preserving addition also preserve subtraction. This unbundled approach targets structures like natural numbers, multisets, and finitely supported functions before they're bundled into full canonically ordered monoids.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Extended unbundled theory for structures with `ExistsAddOfLE`: proves cancellation (`add_tsub_cancel_of_le`, `tsub_add_cancel_of_le`), injectivity (`tsub_left_inj`, `tsub_inj_right`), associativity variants (`add_tsub_assoc_of_le`, `tsub_tsub_assoc`, `tsub_add_tsub_cancel`), comparison lemmas (`tsub_le_tsub_iff_right`, `tsub_lt_iff_left`, `le_tsub_iff_le_tsub`), and extensive `AddLECancellable`-specific results for fine-grained control when only certain elements satisfy cancellation properties; also includes order-reflecting variants for structures with `AddLeftReflectLE` and `AddLeftReflectLT` |
| Hom.lean | Homomorphism theory for ordered subtraction: proves `AddHom.le_map_tsub` showing additive homomorphisms weakly preserve tsub (`f a - f b ≤ f (a - b)`), `map_tsub_of_le` for exact preservation when the second argument is at most the first (`f a - f b = f (a - b)` for `b ≤ a`), `OrderIso.map_tsub` showing order isomorphisms that preserve addition also preserve subtraction exactly, and applications to multiplication in distributive structures (`le_mul_tsub`, `le_tsub_mul`) |

## Subdirectories

*(none)*

## Search Tags

unbundled-canonically-ordered-monoid ordered-subtraction tsub exists-add-of-le add-le-cancellable cancellation associativity injectivity comparison-lemmas homomorphism-preservation order-isomorphism additive-homomorphism monotone-homomorphism weak-preservation exact-preservation multiplication-distribution add-left-reflect natural-numbers multiset finitely-supported-functions