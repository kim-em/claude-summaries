---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Field
generated: 2025-12-01T20:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 15
subdirs_count: 2
---

# Field

## Overview

The `Field/` directory represents the pinnacle of the mathlib4 algebraic hierarchy, defining division rings and fields—structures where every nonzero element has a multiplicative inverse. It provides the fundamental type classes (`DivisionSemiring`, `DivisionRing`, `Semifield`, `Field`) and the predicate-based `IsField` for rings satisfying field axioms. Beyond structural definitions, the directory develops rich theory including division arithmetic, rational casting, geometric series, periodic functions, and instance transfer mechanisms across equivalences and opposites. Two subdirectories extend this foundation: `Action/` develops conjugation actions of division rings on themselves, while `Subfield/` provides bundled subfield types with complete lattice structure and closure operations for working with sub-division rings.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core type class definitions for `DivisionSemiring`, `DivisionRing`, `Semifield`, and `Field` with rational casting and scalar multiplication operations |
| Basic.lean | Fundamental lemmas about division in division semirings/rings and fields (addition/subtraction of fractions, inverse operations, pullback constructions) |
| IsField.lean | `IsField` predicate on semirings (existence-based, no data) and conversions between `IsField` and field structures |
| MinimalAxioms.lean | Constructor `Field.ofMinimalAxioms` to define field structure from minimal axiom set (7 laws + nontriviality) |
| Equiv.lean | Transfer field structures across ring isomorphisms via `MulEquiv.isField` and `IsLocalHom.isField` |
| Rat.lean | Field instance on ℚ (rational numbers) and semifield instance on ℚ≥0 (nonnegative rationals) |
| GeomSum.lean | Geometric series formulas in division rings and fields: `∑ xⁱ = (xⁿ-1)/(x-1)` and bivariate variants |
| Periodic.lean | Periodic and antiperiodic function theory over fields (scaling by field elements, existence in intervals) |
| Power.lean | Results about integer powers in division rings, particularly odd power properties of negation |
| NegOnePow.lean | Integer powers of -1 in division rings: `Int.negOnePow` equals `(-1)^n` |
| Opposite.lean | Field instances for `MulOpposite` and `AddOpposite` types |
| ULift.lean | Field instances for universe-lifted types `ULift α` |
| TransferInstance.lean | Transfer field structures across arbitrary equivalences `α ≃ β` |
| Shrink.lean | Transfer field structures to `Shrink α` (small version in lower universe) |
| ZMod.lean | Field instance for `ZMod p` when p is prime |

## Subdirectories

- [x] `Action/` - Conjugation action theory for division rings with DistribMulAction instances making conjugation compatible with additive and multiplicative structures
- [x] `Subfield/` - Bundled subfield type for division rings, implementing sub-division rings (skew fields) as subrings closed under inverses, with complete lattice structure, closure operations, map/comap along ring homomorphisms, and Galois insertion properties

## Search Tags

field division-ring semifield division-semiring division skewfield rational-numbers rat geometric-series periodic-functions isfield minimal-axioms zmod-field transfer-instance opposite ulift equiv
