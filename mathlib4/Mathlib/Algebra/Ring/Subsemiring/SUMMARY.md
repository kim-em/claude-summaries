---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring/Subsemiring
generated: 2025-12-01T19:50:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 5
subdirs_count: 0
---

# Subsemiring

## Overview

The `Subsemiring/` directory defines bundled subsemirings as subsets of semirings that are closed under both addition and multiplication (with 0 and 1). This implements the complete theory of subsemirings including the `SubsemiringClass` type class, lattice operations (complete lattice structure), ring homomorphism operations (comap, map, range), and specialized constructions like center, centralizer, and opposite semiring equivalences. The files also establish ordered subsemiring instances and pointwise scalar actions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `AddSubmonoidWithOneClass`, `SubsemiringClass` type class, bundled `Subsemiring` structure (combining `Submonoid` and `AddSubmonoid`), basic instances (semiring structure, subtype homomorphism), and conversions to/from `NonUnitalSubsemiring` |
| Basic.lean | Comprehensive subsemiring theory: complete lattice structure (⊤, ⊥, ⊔, ⊓, sSup, sInf), comap/map operations along ring homomorphisms, range of ring homomorphisms (`rangeS`), big operators (list/multiset/finset sums and products), center and centralizer subsemirings, and `topEquiv` isomorphism |
| MulOpposite.lean | Opposite subsemiring constructions: equivalence between subsemirings of `R` and `Rᵐᵒᵖ` via `op`/`unop` operations, lattice-preserving isomorphism `opEquiv`, closure operations, and ring equivalences (`addEquivOp`, `ringEquivOpMop`, `mopRingEquivOp`) |
| Order.lean | Ordered subsemiring instances: `IsOrderedRing` and `IsStrictOrderedRing` instances for `SubsemiringClass` and `Subsemiring`, and `nonneg` subsemiring (nonnegative elements in ordered semirings) |
| Pointwise.lean | Pointwise scalar action: `MulAction M (Subsemiring R)` for `MulSemiringAction M R`, implemented via mapping by `MulSemiringAction.toRingHom`, with lemmas for smul membership, covariance, and interaction with lattice operations (available in `Pointwise` locale) |

## Subdirectories

(none)

## Search Tags

subsemiring bundled-subsemiring subsemiring-class additive-submonoid multiplicative-submonoid closure lattice complete-lattice comap map range center centralizer opposite-ring mul-opposite ordered-subsemiring pointwise-action scalar-action ring-homomorphism semiring
