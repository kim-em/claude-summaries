---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Int
generated: 2025-12-09T09:53:31Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: preliminary
files_count: 23
subdirs_count: 3
---

# Int

## Overview

The `Int/` directory provides comprehensive theories and operations for integers (ℤ) in Mathlib. It includes foundational definitions and lemmas (Init.lean, Basic.lean), number-theoretic operations (GCD, modular arithmetic, divisibility), bitwise operations, logarithms, ordering properties, and specialized constructs like absolute values, intervals, and congruences. The directory serves as the core integer theory layer, extending Lean's built-in Int type with mathematical properties needed for algebra, number theory, and analysis.

## Key Files

| File | Purpose |
|------|---------|
| Notation.lean | Defines the notation `ℤ` for the Int type |
| Init.lean | Basic foundational lemmas about integers that don't depend on Mathlib (can be upstreamed to Batteries); includes succ/pred, induction principles, strongRec, division/modulo basics |
| Basic.lean | Core integer operations and lemmas building on Init.lean; includes natAbs properties, divisibility, and GCD operations |
| GCD.lean | Extended GCD algorithm (Bézout's lemma), computing `a, b` such that `gcd x y = x*a + y*b`; includes divisibility theory and coprimality |
| ModEq.lean | Congruence relation `a ≡ b [ZMOD n]` for integers; modular arithmetic operations and properties |
| DivMod.lean | Additional lemmas about division and modulo (ediv, fdiv, emod) |
| Lemmas.lean | Miscellaneous integer lemmas requiring additional imports beyond Basic; natAbs comparisons, bitwise lemmas, div/mod uniqueness |
| Bitwise.lean | Bitwise operations (div2, bodd, bit, bitwise function application); described as "possibly only of archaeological significance" |
| Log.lean | Integer-valued logarithms in fields: `Int.log` (floor log) and `Int.clog` (ceiling log) with respect to natural base |
| Interval.lean | Proves ℤ is a LocallyFiniteOrder; defines finite intervals (Icc, Ico, Ioc, Ioo) and their cardinalities |
| Range.lean | Integer ranges `range m n` enumerating [m, n) as lists; includes decidability instances for bounded quantifiers |
| AbsoluteValue.lean | Interaction between absolute values and integers; shows absolute values send ℤ units to 1 |
| Associated.lean | Associated elements in the integers (elements differing by a unit) |
| CharZero.lean | CharZero instance and properties for integers |
| ConditionallyCompleteOrder.lean | Conditionally complete lattice structure on integers |
| LeastGreatest.lean | Least and greatest element operations in integer sets |
| NatAbs.lean | Additional properties of natural absolute value natAbs |
| NatPrime.lean | Prime number properties for integers |
| Sqrt.lean | Integer square root function |
| Star.lean | Star operation (involution) on integers |
| SuccPred.lean | Successor and predecessor operations with SuccOrder instance |
| WithZero.lean | WithZero construction for integers |
| CardIntervalMod.lean | Cardinality of integer intervals modulo operations |

## Subdirectories

- [x] `Cast/` - Type casting operations for integers
- [x] `Fib/` - Fibonacci numbers on integers
- [x] `Order/` - Ordering and lattice properties of integers

## Search Tags

integers number-theory gcd modular-arithmetic divisibility congruence bitwise logarithm intervals absolute-value bezout extended-gcd floor-log ceiling-log modulo division nat-abs coprime prime-numbers
