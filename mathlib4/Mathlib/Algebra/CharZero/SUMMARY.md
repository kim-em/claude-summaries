---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/CharZero
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# CharZero

## Overview

The `CharZero/` directory defines characteristic zero for algebraic structures. A ring R has characteristic zero if the natural number homomorphism ℕ → R is injective, meaning every natural number maps to a distinct element. Unlike `CharP R 0` which only requires non-zero naturals map to non-zero elements, `CharZero R` requires full injectivity. The directory provides the core typeclass definition, proves that characteristic zero structures are infinite, establishes quotient theory for division rings, and provides mechanisms to transport the characteristic zero property across injective additive monoid homomorphisms.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `CharZero` typeclass definition requiring `Nat.cast` to be injective, with fundamental lemmas: cast injectivity (`Nat.cast_inj`), zero/one detection (`cast_eq_zero`, `cast_eq_one`), and `NeZero` instances for all natural number casts in characteristic zero structures |
| Infinite.lean | Proves characteristic zero structures are infinite via `CharZero.infinite` instance, using the injective natural number embedding |
| Quotient.lean | Quotient theory for characteristic zero division rings: characterizes when scalar multiples lie in cyclic subgroups (`zsmul_mem_zmultiples_iff_exists_sub_div`) and when quotient scalar multiples are equal (`zmultiples_zsmul_eq_zsmul_iff`), both with explicit modular decompositions using `Fin z.natAbs` |
| AddMonoidHom.lean | Provides `CharZero.of_addMonoidHom` to transport characteristic zero across injective additive monoid homomorphisms that preserve 1, enabling transfer of the property through structure-preserving maps |

## Subdirectories

*(No subdirectories)*

## Search Tags

characteristic-zero charzero injective-cast natural-numbers infinite quotient-groups division-rings additive-monoids type-class algebra
