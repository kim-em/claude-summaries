---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/ENat
generated: 2025-12-09T10:30:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 5
subdirs_count: 0
---

# ENat

## Overview

The `ENat/` directory implements extended natural numbers `ℕ∞ = WithTop ℕ`, which are natural numbers augmented with an infinity element `⊤`. This type is used throughout mathlib for cardinalities, suprema, and other contexts where "unbounded" natural values are needed. The implementation provides the full algebraic structure (commutative semiring with order), lattice operations (suprema/infima), and specialized operations like lifting between finite and infinite values, conversion to/from regular naturals, and exponentiation by extended naturals.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `ENat` as `WithTop ℕ` with notation `ℕ∞`; includes `NatCast` instance and custom recursor `recTopCoe` for pattern matching on `⊤` vs natural casts |
| Basic.lean | Main algebraic instances and operations: semiring structure, order instances, arithmetic operations (`add`, `mul`, `sub`, `pow`), conversions (`toNat`, `lift`), injectivity lemmas, and fundamental properties distinguishing finite from infinite values |
| Lattice.lean | Complete linear order structure, supremum/infimum operations for indexed families and sets, distributivity lemmas for arithmetic over suprema/infima, and finiteness characterizations based on suprema |
| BigOperators.lean | Finite sum operations interacting with suprema; `sum_iSup` exchanges summation with indexed supremum under directedness conditions |
| Pow.lean | Exponentiation of extended naturals by extended naturals (`x ^ y` where both are `ℕ∞`); defines `0 ^ ⊤ = 0`, `1 ^ ⊤ = 1`, `x ^ ⊤ = ⊤` for `x > 1`, with monotonicity and algebraic laws |

## Subdirectories

(none)

## Search Tags

extended-natural-numbers enat WithTop infinity cardinality supremum infimum lattice complete-linear-order arithmetic semiring exponentiation conversion toNat lift
