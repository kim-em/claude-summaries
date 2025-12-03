---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Invertible
generated: 2025-12-01T22:15:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Invertible

## Overview

The `Invertible/` directory defines a typeclass for elements with two-sided multiplicative inverses in contexts where a general inverse operator may not exist. Unlike the `Prop`-valued `IsUnit`, `Invertible` is a `Type`-valued construction that enables computations with inverses in structures like `ℤ[1/2]` where only some elements are invertible, or for specifying that a field has characteristic `≠ 2`. The typeclass provides the notation `⅟a` for the inverse and establishes the bidirectional connection with units: every invertible element corresponds to a unit, and every unit is invertible.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `Invertible` typeclass definition with inverse element `⅟a` notation; defines basic properties (`invOf_mul_self`, `mul_invOf_self`), cancellation lemmas, inverse uniqueness, and fundamental constructions including `invertibleOne`, `invertibleInvOf`, and `invertibleMul` |
| Basic.lean | Theorems connecting invertibility to units and `IsUnit`; defines `unitOfInvertible` and `Units.invertible` conversions, commutativity properties of inverses, derived constructions (`invertibleOfInvertibleMul`, `invertibleOfMulInvertible`, `invertiblePow`), and monoid homomorphism preservation of invertibility |

## Subdirectories

(none)

## Search Tags

invertible inverse invOf units two-sided-inverse typeclass multiplicative-inverse computation half third fraction characteristic monoid group isUnit cancellation commute power monoid-homomorphism
