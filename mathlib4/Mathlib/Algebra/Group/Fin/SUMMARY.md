---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Fin
generated: 2025-12-01T22:00:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Fin

## Overview

The `Fin/` directory provides algebraic group structures and properties for finite types `Fin n`, representing the integers modulo n. It establishes `Fin n` as an additive commutative group (when n is nonzero) with comprehensive theory for addition, subtraction, negation, and related operations, along with specialized lemmas for tuple operations on function types `Fin n → α`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core algebraic instances for `Fin n`: `AddCommSemigroup`, `AddCommMonoid` (when `NeZero n`), `AddCommGroup` (when `NeZero n`), `InvolutiveNeg`, and cancellation properties; includes specialized lemmas for subtraction (`coe_sub_one`, `lt_sub_iff`), bounds (`lt_one_iff`, `le_sub_one_iff`), negation (`neg_last`), reversal operations (`rev_add`, `rev_sub`), and addition properties |
| Tuple.lean | Algebraic properties of tuples (functions `Fin (n+1) → α`): `insertNth` operations for multiplication/division, scalar multiplication on vectors via `Matrix` namespace, and pointwise operations (add/sub/zero/neg) on `vecCons`, `vecHead`, `vecTail` for building and manipulating finite tuples with group structure |

## Subdirectories

(none)

## Search Tags

fin finite-type modular-arithmetic additive-group additive-commutative-group tuple vector algebraic-operations insertion cancellation involutive-negation nat-cast
