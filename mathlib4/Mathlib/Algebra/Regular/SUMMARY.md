---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Regular
generated: 2025-12-04T15:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Regular

## Overview

The `Regular/` directory defines regular elements in algebraic structures and their properties. A regular element is one where multiplication (or scalar multiplication) by that element is injective. The theory includes left-regular, right-regular, and fully regular elements, with both multiplicative variants (`IsLeftRegular`, `IsRightRegular`, `IsRegular`) and their additive analogues. The directory also introduces `IsSMulRegular` for module-theoretic regularity, generalizing the concept to scalar actions. This is foundational for understanding non-zero divisors in commutative rings and cancellation properties in algebraic structures.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `IsLeftRegular c` (multiplication by `c` on left is injective), `IsRightRegular c` (multiplication by `c` on right is injective), and `IsRegular c` (both left and right regular), with additive analogues |
| Basic.lean | Fundamental theory of regular elements: interaction with commuting elements, closure under products in semigroups, units are regular, powers of regular elements are regular, characterization in terms of `1`, and proof that `0` is regular iff structure is trivial in `MulZeroClass` |
| SMul.lean | Module-theoretic regularity via `IsSMulRegular M c` (scalar multiplication by `c` is injective on `M`), generalizing `IsLeftRegular` to arbitrary module actions, with theory for scalar towers, units, groups, and equivalence characterizations |
| Opposite.lean | Behavior under `MulOpposite`: `IsLeftRegular (op a) ↔ IsRightRegular a`, `IsRightRegular (op a) ↔ IsLeftRegular a`, and `IsRegular (op a) ↔ IsRegular a` |
| Pi.lean | Regularity in dependent function types: element is regular iff regular componentwise, `IsLeftRegular a ↔ ∀ i, IsLeftRegular (a i)`, and analogues for right-regular, regular, and `IsSMulRegular` |
| Pow.lean | Finite products of regular elements: `IsLeftRegular.prod`, `IsRightRegular.prod`, `IsRegular.prod` for products over finsets in commutative monoids |
| Prod.lean | Regularity in product types: `IsLeftRegular (a, b) ↔ IsLeftRegular a ∧ IsLeftRegular b` and analogues for right-regular, regular, and `IsSMulRegular` |
| ULift.lean | Regularity preserved under universe lifting: `IsLeftRegular (up a) ↔ IsLeftRegular a` and analogues for `down`, right-regular, regular, and `IsSMulRegular` |

## Subdirectories

None

## Search Tags

regular-elements left-regular right-regular is-regular non-zero-divisors cancellation injective-multiplication scalar-regular smul-regular module-action opposite-algebra product-types pi-types universe-lifting commutative-semigroup monoid units powers finset-product
