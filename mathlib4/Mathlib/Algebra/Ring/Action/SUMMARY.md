---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring/Action
generated: 2025-12-01T21:42:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 9
subdirs_count: 1
---

# Action

## Overview

The `Action/` directory defines the theory of multiplicative actions by monoids and groups on rings and semirings. The central typeclass is `MulSemiringAction`, which combines distributive actions with multiplicative compatibility, expressing how a monoid acts on a semiring while preserving both addition and multiplication. This framework is essential for formalizing algebraic structures like Galois group actions on field extensions, conjugation actions by units, and automorphism group actions. The directory also provides the `Pointwise/` subdirectory establishing how these scalar actions interact with pointwise operations on sets and finite sets in ring-theoretic contexts.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `MulSemiringAction` typeclass: monoids acting on semirings with `g • (x + y) = (g • x) + (g • y)` and `g • (x * y) = (g • x) * (g • y)`, conversion to ring homomorphisms |
| Group.lean | Ring automorphisms from group actions: `MulSemiringAction.toRingEquiv` converting group elements to ring isomorphisms |
| End.lean | Ring automorphism group structure: `RingAut R` acts on `R` via `MulSemiringAction`, with conversion `MulSemiringAction.toRingAut` |
| ConjAct.lean | Conjugation action on rings: units act on the ring via conjugation `u • r = u * r * u⁻¹` |
| Field.lean | Field-specific action properties: scalar multiplication commutes with inversion `x • m⁻¹ = (x • m)⁻¹` |
| Invariant.lean | Invariant subrings: `IsInvariantSubring` typeclass for subrings fixed elementwise by a `MulSemiringAction`, with induced action on the subring |
| Rat.lean | Rational number scalar actions: `DistribSMul` instances for `ℚ≥0` and `ℚ` acting on division (semi)rings |
| Submonoid.lean | Fixed point substructures: additive submonoid/subgroup of elements fixed under the entire action |
| Subobjects.lean | `MulSemiringAction` instances for submonoids and subgroups: subobjects inherit actions from ambient monoids/groups |

## Subdirectories

- [x] `Pointwise/` - Pointwise scalar actions on sets and finite sets: negation compatibility with scalar multiplication in ring modules

## Search Tags

mul-semiring-action group-action ring-action semiring-action distributive-action galois-action automorphism ring-automorphism ring-equivalence conjugation invariant-subring fixed-points scalar-multiplication
