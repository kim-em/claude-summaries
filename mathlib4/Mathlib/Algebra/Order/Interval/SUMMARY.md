---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Interval
generated: 2025-12-01T22:10:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 2
---

# Interval

## Overview

The `Interval/` directory provides a comprehensive framework for interval arithmetic and operations across different mathematical container types. It implements full-precision arithmetic (addition, multiplication, powers, subtraction, division, negation) on abstract interval types (`NonemptyInterval α`, `Interval α`) with correctness proofs under monotonicity assumptions. The directory systematically develops algebraic properties for interval representations over three container types: finite sets (Finset.Ixx), multisets (Multiset.Ixx), and general sets (Set.Ixx). The Finset subdirectory focuses on translation operations and successor-predecessor relations in locally finite orders. The Set subdirectory provides the most comprehensive treatment, including group/monoid operations, bijective translations, algebraic instances for unit intervals [0,1], pairwise disjointness lemmas, and successor-predecessor equivalences. This infrastructure supports applications in analysis, optimization, and verified computation with intervals.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core interval arithmetic: defines algebraic operations (one/zero, multiplication/addition, powers, subtraction, division, negation/inversion) on `NonemptyInterval α` and `Interval α` types with proofs of correctness under monotonicity assumptions; includes interval length and positivity extensions |
| Multiset.lean | Algebraic properties of multiset intervals: proves that left/right addition maps (`map (c + ·)`, `map (· + c)`) on `Multiset.Ixx` intervals (Icc, Ico, Ioc, Ioo) translate endpoints correctly for ordered cancel additive monoids |

## Subdirectories

- [x] `Finset/` - Translation of finset intervals under addition and successor-predecessor relations in locally finite orders (complete)
- [x] `Set/` - Group/monoid operations on set intervals, bijective translations, unit interval [0,1] algebraic instances, and successor-predecessor equivalences (complete)

## Search Tags

interval-arithmetic nonempty-interval interval-type algebraic-operations interval-multiplication interval-addition interval-powers interval-subtraction interval-division finset-intervals multiset-intervals set-intervals unit-intervals ordered-monoids ordered-groups monotonicity interval-length
