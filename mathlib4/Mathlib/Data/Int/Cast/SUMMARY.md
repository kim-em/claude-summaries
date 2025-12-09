---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Int/Cast
generated: 2025-12-09T10:51:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 6
subdirs_count: 0
---

# Cast

## Overview

The `Cast/` directory provides the canonical coercion (cast) from integers (ℤ) to various algebraic structures, particularly rings and fields. It defines the fundamental type classes `AddGroupWithOne` and `AddCommGroupWithOne` that enable this casting, along with comprehensive lemmas about how integer casts interact with algebraic operations, homomorphisms, and specialized type constructors like products, Pi types, and fields. This is the foundation for using integer literals in arbitrary mathematical structures.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `Int.castDef` default implementation, `AddGroupWithOne` type class (enabling `ℤ → R` homomorphism), and `AddCommGroupWithOne` for commutative structures |
| Basic.lean | Additional cast theorems beyond Defs; includes `cast_negSucc`, `cast_zero`, `cast_natCast`, `cast_one`, `cast_neg`, `cast_add`, `cast_sub`, and helper lemmas for natural number casts |
| Lemmas.lean | Advanced properties involving algebraic homomorphisms and order structure: `castAddHom` and `castRingHom` bundled homomorphisms, injectivity in `CharZero`, commutativity lemmas, `zsmul_eq_mul` identity, divisibility preservation, extensionality for homomorphisms from ℤ, and `zmultiplesHom`/`zpowersHom` equivalences |
| Field.lean | Integer cast properties in division rings and fields; main result: `Int.cast_div` showing `↑(m / n) = ↑m / ↑n` when `n ∣ m` |
| Pi.lean | Pointwise integer cast for function types: `Pi.instIntCast` mapping `n : ℤ` to the constant function `fun i => n`; includes simp lemmas for application and definition forms |
| Prod.lean | Integer cast for product types: `AddGroupWithOne (α × β)` instance where `(n : α × β) = (n, n)`; includes projection simp lemmas |

## Subdirectories

*(none)*

## Search Tags

integer-cast coercion type-class addgroupwithone canonical-homomorphism ring-homomorphism cast-lemmas charzer injective algebraic-homomorphisms zsmul field-cast division product-types pi-types function-cast commutativity extensionality
