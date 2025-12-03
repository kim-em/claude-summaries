---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Floor
generated: 2025-12-01T20:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 6
subdirs_count: 0
---

# Floor

## Overview

The `Floor/` directory implements floor and ceiling functions for ordered algebraic structures. It provides two main type systems: `FloorSemiring` for natural-valued floor/ceil (⌊a⌋₊, ⌈a⌉₊) on ordered semirings, and `FloorRing` for integer-valued floor/ceil (⌊a⌋, ⌈a⌉) on linearly ordered rings. The theory is developed through a hierarchy of files: core definitions and typeclasses (Defs), basic semiring lemmas (Semiring), specialized semifield results (Semifield), comprehensive ring theory with fractional parts (Ring), specialized division operators for ordered monoid actions (Div), and extended floor/ceil functions for ℝ≥0∞ → ℕ∞ (Extended). The implementation includes Galois connection characterizations, monotonicity results, `positivity` and `norm_num` tactic extensions, and practical applications like integer division properties.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclasses `FloorSemiring` and `FloorRing` with Galois connection axioms; defines Nat.floor/ceil (⌊a⌋₊, ⌈a⌉₊) and Int.floor/ceil/fract (⌊a⌋, ⌈a⌉); provides constructors `FloorRing.ofFloor` and `FloorRing.ofCeil` for building instances from single functions |
| Semiring.lean | Lemmas for Nat.floor/ceil on ordered semirings: monotonicity, interaction with natural casting, characterizations (floor_eq_iff, ceil_eq_zero), preimage descriptions for floor function |
| Semifield.lean | Division properties for Nat.floor/ceil in semifields: floor_div_natCast relates floor of quotient to quotient of floors, inequalities for multiplication bounds (mul_lt_floor, ceil_lt_mul, div_two_lt_floor), `norm_num` extension for computing floor of concrete rationals |
| Ring.lean | Comprehensive Int.floor/ceil/fract theory (700+ lines): floor/ceil characterizations and inequalities, monotonicity and interaction with arithmetic, fractional part properties (0 ≤ fract < 1), conversion between Int and Nat floor/ceil functions, `positivity` extensions for automated positivity reasoning |
| Div.lean | Flooring and ceiling division operators for ordered monoid actions: typeclasses `FloorDiv` (b ⌊/⌋ a) and `CeilDiv` (b ⌈/⌉ a) characterized by Galois connections, instances for ℕ, Pi types, and Finsupp; intended for finding adjoints to scalar multiplication b ↦ a • b |
| Extended.lean | Extended floor/ceil functions ENat.floor, ENat.ceil : ℝ≥0∞ → ℕ∞ with notation ⌊r⌋ₑ, ⌈r⌉ₑ; handles top element (∞ maps to ⊤), Galois connection characterizations, arithmetic interaction (floor/ceil commute with addition/subtraction of naturals), monotonicity, and `positivity` extension for ENat.ceil |

## Subdirectories

(none)

## Search Tags

floor ceiling round fract FloorSemiring FloorRing galois-connection monotonicity ordered-semiring ordered-ring integer-valued natural-valued fractional-part division-operators extended-naturals positivity norm-num tactic-extensions
