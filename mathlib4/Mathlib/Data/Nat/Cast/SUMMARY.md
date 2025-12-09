---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/Cast
generated: 2025-12-09T10:42:38Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: preliminary
files_count: 9
subdirs_count: 1
---

# Cast

## Overview

The `Cast/` directory implements the canonical homomorphism from natural numbers (ℕ) to arbitrary algebraic structures with addition and one. It defines the fundamental type classes `NatCast` and `AddMonoidWithOne` that enable numeric literals (like `37 : R`) to work in any ring or monoid. The directory provides both unary and binary casting algorithms, proves that `Nat.cast` is a ring homomorphism, and establishes properties about casting in various contexts including fields, products, order duals, and specialized situations like commutativity and nonzero elements.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `NatCast` type class, `AddMonoidWithOne` structure, `Nat.unaryCast` and `Nat.binCast` algorithms, foundational lemmas about `cast_zero`, `cast_succ`, `cast_add` |
| Basic.lean | Additional theorems about `Nat.cast`: bundled homomorphisms (`castAddMonoidHom`, `castRingHom`), multiplication and power lemmas, extensionality results, and uniqueness of ring homomorphisms from ℕ |
| Field.lean | Casting into fields (`DivisionSemiring`): `cast_div` lemma showing `↑(m / n) = ↑m / ↑n` when `n ∣ m`, with specialized versions for `CharZero` fields |
| Commute.lean | Commutativity lemmas: proves natural number casts commute with all elements (`Nat.cast_commute`), semiconjugacy properties for natural multiples |
| NeZero.lean | Properties of nonzero casts: `NeZero.natCast_ne` establishes that `NeZero (n : R)` implies `(n : R) ≠ 0`, bidirectional implications between `NeZero n` and `NeZero (n : R)` |
| Prod.lean | Product instances: `AddMonoidWithOne` structure for `α × β`, component-wise casting with `fst_natCast` and `snd_natCast` lemmas |
| Synonym.lean | Type synonym instances: `NatCast` and `AddMonoidWithOne` for order dual (`αᵒᵈ`) and lexicographic order (`Lex α`), with conversion lemmas |
| SetInterval.lean | Set interval images under `Nat.cast : ℕ → ℤ`: proves that casting intervals `Ixx a b` from ℕ to ℤ produces the corresponding integer intervals, range characterization |
| WithTop.lean | Casting to `WithTop ℕ` and `WithBot ℕ`: `Nat.cast_withTop` and `Nat.cast_withBot` lemmas, well-founded relation instance |

## Subdirectories

- [ ] `Order/` - Order-theoretic properties of natural number casts

## Search Tags

nat-cast coercion homomorphism AddMonoidWithOne numeric-literals ring-hom field-cast commute nonzero type-class
