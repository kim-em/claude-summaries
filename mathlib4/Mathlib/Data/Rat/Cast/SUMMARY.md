---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Rat/Cast
generated: 2025-12-11T21:45:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 5
subdirs_count: 0
---

# Cast

## Overview

The `Cast/` directory contains lemmas about casting rational numbers (ℚ and ℚ≥0) into other algebraic structures. It defines the canonical injection from rationals into division rings/semirings, proves that these casts are well-behaved ring homomorphisms, establishes order-preserving properties into ordered fields, and provides `norm_cast` simp lemmas for arithmetic operations. The files also include `positivity` tactic extensions for rational casts and the `LawfulOfScientific` instance for characteristic zero fields.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core casting definitions: `Rat.cast_def`, `NNRat.cast_def`; casting of ℕ, ℤ literals; commutativity of casts; `norm_cast` lemmas for add/sub/mul/div/inv when denominators are non-zero; extension lemmas for `MonoidWithZeroHom` showing homs from ℚ or ℚ≥0 are determined by their action on integers/naturals; `Subsingleton (ℚ →+* R)` |
| CharZero.lean | Cast injectivity in characteristic zero: `cast_injective`, `cast_inj`, `cast_eq_zero`; unconditional `norm_cast` lemmas for +/-/*/inv/div/zpow when target has CharZero; `Rat.castHom` and `NNRat.castHom` as ring homomorphisms |
| Order.lean | Order-preserving cast lemmas for linear ordered fields: `cast_strictMono`, `cast_mono`, `castOrderEmbedding`; comparison lemmas (`cast_le`, `cast_lt`, `cast_nonneg`, `cast_pos`); preimage lemmas for intervals (Icc, Ico, Ioi, etc.); `positivity` tactic extensions for `Rat.cast` and `NNRat.cast` |
| Lemmas.lean | Additional casting lemmas: `cast_pow` for natural exponents; `cast_inv_nat`, `cast_inv_int` for inverses; `cast_nnratCast` relating ℚ≥0 → ℚ → K to ℚ≥0 → K; `cast_ofScientific` showing scientific literal casting commutes with rational cast |
| OfScientific.lean | `LawfulOfScientific K` instance for characteristic zero fields, ensuring scientific notation literals behave correctly with field operations |

## Subdirectories

*(none)*

## Search Tags

rational-cast cast-homomorphism norm-cast char-zero order-embedding strict-mono injective castHom positivity scientific-notation nnrat rat division-ring
