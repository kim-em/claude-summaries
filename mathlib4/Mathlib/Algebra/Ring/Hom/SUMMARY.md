---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring/Hom
generated: 2025-12-01T20:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Hom

## Overview

The `Hom/` directory contains the fundamental definitions and theory of ring homomorphisms and non-unital ring homomorphisms. This includes the core bundled structures `RingHom` (notation `→+*`) and `NonUnitalRingHom` (notation `→ₙ+*`), their associated type classes (`RingHomClass` and `NonUnitalRingHomClass`), basic operations (identity, composition), and properties (injectivity-based domain transfers). The module also provides constructors for building ring homomorphisms from monoid homomorphisms or additive homomorphisms under various conditions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of `NonUnitalRingHom` (additive monoid homomorphisms preserving multiplication) and `RingHom` (monoid homomorphisms preserving addition), with their type classes, coercions, basic operations (identity, composition, zero), instances (monoid structure on endomorphisms), and alternative constructors like `RingHom.mk'` and `AddMonoidHom.mkRingHomOfMulSelfOfTwoNeZero` |
| Basic.lean | Deprecated module (since 2025-06-09) that re-exports `InjSurj` and deprecated ring homomorphism functionality |
| InjSurj.lean | Pullback of `IsDomain` instance along injective ring homomorphisms: if `f : β →*₀ α` is injective and `α` is an integral domain, then `β` is also an integral domain |

## Subdirectories

None.

## Search Tags

ring-homomorphism semiring-homomorphism non-unital-ring-hom RingHom NonUnitalRingHom bundled-hom ring-hom-class composition identity map-zero map-one map-add map-mul injective domain pullback
