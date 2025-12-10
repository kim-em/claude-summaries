---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Num
generated: 2025-12-11T09:45:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 5
subdirs_count: 0
---

# Num

## Overview

Binary representation of natural numbers and integers using inductive types. This module provides `PosNum` (positive binary numbers), `Num` (non-negative binary numbers), `ZNum` (signed binary integers), and `SNum` (signed integers using two's complement bit strings). Unlike Lean's native Peano-style `Nat`, these representations store numbers in binary form (e.g., 13 = 1101 in base 2 = `bit1 (bit0 (bit1 one))`). While discouraged for general use (prefer `Nat` and `Int`), these types are useful for kernel computation contexts like proofs by `rfl`, `decide`, and `#reduce`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core type definitions (`PosNum`, `Num`, `ZNum`) with basic arithmetic operations (successor, addition, multiplication, comparison, division, modulo, GCD) and coercions to other numeric types |
| Bitwise.lean | Bitwise operations (or, and, xor, ldiff, shift left/right, testBit) for `PosNum` and `Num`, plus `SNum`/`NzsNum` types for two's complement signed arithmetic |
| Lemmas.lean | Extensive proofs relating binary representations to `Nat`/`Int`: casting lemmas, arithmetic correctness, order instances (`LinearOrder`, `CommSemiring`, `IsStrictOrderedRing`), and transfer tactics |
| Prime.lean | Primality testing for `Num` and `PosNum` using binary `minFac` algorithm; decidable `Prime` predicate optimized for kernel computation rather than VM evaluation |
| ZNum.lean | Properties of `ZNum` (signed binary integers): casting, arithmetic, order instances (`CommRing`, `LinearOrder`, `IsStrictOrderedRing`), division/modulo, GCD, and transfer tactics for proof automation |

## Subdirectories

(none)

## Search Tags

binary-numbers posnum num znum snum bitwise kernel-computation binary-arithmetic primality transfer-tactics two's-complement
