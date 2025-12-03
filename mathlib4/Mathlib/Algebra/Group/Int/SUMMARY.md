---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Int
generated: 2025-12-01T22:45:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Int

## Overview

The `Int/` directory provides integer-specific group-theoretic constructions and properties. It establishes the integers as an additive commutative group and multiplicative commutative monoid, defines parity (even/odd) predicates and related lemmas, characterizes units (invertible elements) in the integers, and provides utilities for working with the `Multiplicative ℤ` type tag. This directory serves as the concrete instantiation of abstract group theory for the fundamental integer type.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclass instances making integers an `AddCommGroup` and `CommMonoid`; includes `nsmul` and `zsmul` definitions, torsion-freeness, and short-circuit instances to prevent non-computable instance usage |
| Even.lean | Parity theory for integers; defines `Even` predicate, decidability instances for `Even` and `IsSquare`, parity lemmas for arithmetic operations (add, sub, mul, pow), and the `parity_simps` simp set |
| TypeTags.lean | Conversions and lemmas for `Multiplicative ℤ`; relates additive operations on `ℤ` to multiplicative operations on `Multiplicative ℤ` via `toAdd`, `ofAdd`, and power operations |
| Units.lean | Theory of units (invertible elements) in the integers; proves that units have `natAbs = 1`, characterizes units as exactly `±1`, and provides extensive lemmas about products equaling `±1` |

## Subdirectories

(No subdirectories)

## Search Tags

integer int group additive-group multiplicative-monoid parity even odd units invertible-elements type-tags multiplicative torsion-free decidability arithmetic
